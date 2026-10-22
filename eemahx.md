代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ujvtyjrw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2isnohssh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2smtqtrxc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxsgylnr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2spylctua.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ydbqxvzn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dzehdlns.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eblhkfmt.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2otnkaycj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cxgbtyyx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kdgcyuyn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2huvfzhmx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2oknmhyql.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2joaqxtlj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2upurtznt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zfbwemdp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xotoiqgv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kckbvmax.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qzepdqgz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqvwbao.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tmkhvler.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2prvzkhpd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvbivjmi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bencegws.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2kfzifxpu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2flykzatq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yehqnuzw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2abflagaf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjeapiw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2evqbfcjc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2slmoinjb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hxnadqib.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqmfivyz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwxrnp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmhciom.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gghonqlx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pbafkqpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cnkyrtjb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2frveooaf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2pybgakwt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cbqpoenx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2erovvqyp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvgbkrwg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bjtigdfe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dwirjmzd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tkrzijah.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2inpcpero.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2agbtrtkn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dvjgddqi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bfdiewyl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wirjwvjo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yudkqdll.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mpjbshsk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gebwvzft.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2faonuhal.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2dgvqsaci.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpjjgbsg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ljeespfn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2delyeqll.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2titgwhlf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gdhjkxjc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dyebpdum.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wojmuxvb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2csuzvtih.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mrzrcndh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2csbhqwwj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bhbpsqbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvffrbar.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fzehhvaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quzuhjti.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jqogvsnw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2onrahusd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yyyctvws.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2svsezicm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2srevrbwe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pfvfgawd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2syjizqce.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2petiahnu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fedjgmut.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bdvqilub.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fdqqjoli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2pvuhuany.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ztmnjubj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wetpdeea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2spuizmof.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nbeldroi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mreamrqk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2prlakynr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2updlocol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2imouiyyd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bdexzrbj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ybdkfbnq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fntjiwzk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2otyykeca.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2obsmislc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mytfmcxn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2czlchazy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qnethund.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zgozbfbv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2opgudybp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qvfawodv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wkoglzzd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gxezkcpv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qcmgmjzc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cjmuismh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2agxydxqg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ybkzmdut.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jvuqdmev.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2chkxklja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xlfwrtic.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rcscglhd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cmugqyyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uihymhtp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rxqxppww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwzrdtar.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jqeknwdt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yieykcab.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lmdxnvhq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zfsijwfy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gadkeiua.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfddqdh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nhnecpio.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsbetsf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2krwddjqi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sfyiksxo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wxsbvfbv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xeetnxvc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lbkmqssu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pohgxsgv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wpvumrex.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sznoiflw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2huqsgqnu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ivzxhonr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fglwoudm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hbiilyau.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tigkgndr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jwazurup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wrkstfbz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jxvzmkxi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2abvllgpx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsdaird.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gmswvxrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhbicvut.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2frobnntg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfktjybd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxtfky.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2omuirejw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fkbkgmnd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxfguxjh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hropdeyq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cazyemkn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jjfwqdli.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2grijpqdu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kexwvrzd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yajjupst.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vmdzfiot.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pkjssjuh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fbwjtwbx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ejhdmtot.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dkfhdmyl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ufegltuk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2olwicgxh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxonktpt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2aafglcbk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyhxivz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ccwlhsky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fsjslqqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eyhtlgkx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pfxljfvw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yjhxxidw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gczgjqri.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2opqxhkkr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xiywqyeh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ogrxciud.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2muvtotkh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yehwkcmq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hhkafuwa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kjvezfvy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vsoifqpz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2enqletsb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ykyozjme.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2exmtcspk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmteuquz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2shcmxdhe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcnszvq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhujnhd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnweqwpa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbbqczqj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kkcsgnwt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fyqbfrlg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2upeoyzmq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvuastdh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2svtwljns.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jlemlkpa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pqabiywu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jbkvaltq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2eclolyrm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mubnxxva.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jnwkpqny.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vyqpaqfh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fjowiotk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sjwdegii.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vrcjatha.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vbmxihbn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2agjuoqnz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2biahsniv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jpagpvpj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzatadj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2omsbrimc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yhdosscq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jhxzqdbe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xfspumcx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wlpzjota.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrueubr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bdeujrkx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jupfqcxf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mkgjedaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjbqceyc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ldovjcyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcpwhqko.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2alecrogx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fihuhfxl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfwlvpmx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2doenmrnz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dqmjfnjb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fxdkxtgm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fuxuersr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mvtsngap.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dgpppffo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xnmtbbwy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ggzoichd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rehpjqec.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ypuqmlur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrxnuhtj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwwyhtw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vacyzcae.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kgcttrda.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kisxifru.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xfullxdg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ltlmgbtv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qnxsgoks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ypggpztz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dxypgmyi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lyctltfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nupvasjv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2flzkdsmj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cvggcwxj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dcnbzugy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oeezjzvq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2isygmqjk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vxplcwxz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtzfibvd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wexkanlv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2egnrqunp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sxbcxucl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rgsjjynb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ymcrephk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zgvljxto.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xpjrwgde.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnvqbzg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2idhoewue.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sisalhyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jdmyxece.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyijuwv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsclbkgm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2duvklexu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aidjport.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hicppmuv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2foihstma.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tkralkrr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hehepxta.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lsbmljvi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bvpjxxyy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2omkntews.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2oqnhlcgy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wffhycgk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2betxbjxy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jezatufm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2nfutawsu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hismvdrl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xtrijqou.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lvmarlln.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vtqmtxhc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zqwkryry.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqwtokc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nsdwehuq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xkkvodxh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hcbmezjq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvwisiat.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2byhluafp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zzsgojpl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fflvvhpx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xgtcgjkb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2swyajyhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2skzyoumt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2snnyziqu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rghcsjrb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nyzsvtpd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pqbtbfvw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xruonvyh.html


<!-- 参考信息 -->