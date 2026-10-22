代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2aizbctxp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2uthuzkuw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2omtuwicp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lkpjpuxk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xomuwjxh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cskcucqe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vkkjwwue.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gyiigjwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdocrqg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2iidciqyu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rpnydjxz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cgzdebtq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nnibjwpi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvddjhnm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrecjzk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2krsnllye.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2flbklbky.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xfxehrsw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlqjowil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ehseahzc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qgitlmqr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cmrbfxvv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dimrzucg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsadleo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rfukepgf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbkcuepi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2durtwbry.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jtibfbom.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wduyxubh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2xajupita.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gpcqlokd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmsmty.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qnnqjnzz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rfihbalz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qvbaogib.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2iyqvmlog.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cnhhluxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wbmgsiuc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tegvphff.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tvldovxl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cawggdql.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2egnqwkhp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dertuubu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2djibsjmj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2emgmolku.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nblfsbot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gzltjzqm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2pbarmphe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mgwsttbw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvnunfl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tinnavgm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kbeunpgu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cwcljgkd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tnkvnnrb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ndtptpxb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkwztw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgqvteqo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mhhhpoxx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lpdwcwzq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2acijwzvw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ijdxtfnq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hifqbdly.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uqzrepvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzzkxsio.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2spvxmjst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnsoyhqr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wsebzwel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fbmwqqxo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2csxuaibz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zyrzadzn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hcblexbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mgukggml.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hkrlvuvg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nqlnfark.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dyrjxvqf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aparnnbh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2isbgdnox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bybdrrrw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gsnafcsu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vjkiepdl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rustigey.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kazgwshw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xfitqogt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iprfsiwr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2umhmgxyh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2iydipeuq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2atmuipjf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fbdqgrra.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iibextkn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tiiihymw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xeyhjwin.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2emfeiemt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qsrcdpyl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jtkrpnph.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pftwbhph.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yaszxhmb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2csrbgthl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbdisfbl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hybghfzb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2avwyknpq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bjoqoghl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tswxlnha.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2feadvbnd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jchdqqtf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzltjffa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xmiujudl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vuiuefrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2viaehzkh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ccrlpnle.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wtqusifh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kdjbjqwl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zgffqyai.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mhstxvlv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sqlyzujz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yauwvnqe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kkxzpvkg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xgzbufqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbxfsx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfdctrf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2twoqkrec.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2etrsgrgu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wnwtjtnb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2euscjrke.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gufljqog.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oouadwsn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yncuhnal.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2thwemlsj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bstilwqq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zxjyffzg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2utjrvwxa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dhjbpoir.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ubrqhhus.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2znvyhibi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qeehuocr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hhykfxso.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wzvotazj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mahyvlij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bkrfleqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebnqnpci.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lbcyaxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpspncov.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kdqalmtl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kjxxntuj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hqmtheit.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqciumu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvodeem.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qchzexvu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bpjmsagp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ywtawaxi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jlzzyock.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cllzuaox.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gzsfnzkl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yzyifqtv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ohhwdpah.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jwljpamd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rccovnfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xkhbgenw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zjqyuhdy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fhuodexs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2oyekehcx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2szvdmwyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bjazrqiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdblue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hrrzizcr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iskdcsnf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nhylaurm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2psyvmgpw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ailiheaa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nqyuvedu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjkivnjt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yuakumsw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nclkfhnv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gryufmxt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wwvxjqjt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2umjbwmph.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ucydmisn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mbunfhld.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2eprceivt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqinwjjo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzlnhszz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhndvtrb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mdrnuics.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzalbdy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzmqwsf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dezewhsy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2djwgubwg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2npqhswjv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2heouzsfc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpatow.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ndaffvcy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xezrjuim.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2avsrgnzi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dwmjtghn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dbbwohmd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gieecxzj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fxocshfn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uxzssyll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jdlzucrs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2adnaqiyq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yubmhque.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dhndeimf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qxgevpvn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2abmkccgd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cehuvmdq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2selgntrm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hdbxngpz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2obmhmiwa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2obtivsdy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cydmawrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2migleukq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cpazmyrr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2laabmcum.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tchjcefa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjolelvf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hjpgxwft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjvoyhog.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fbskrcbr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rppzvpgi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gsbldjas.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtqbyhf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnogeog.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvvcxqc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dbeniudz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qstobxis.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdyqospg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jniwrxqb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2heunakuz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lblfqdal.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aurxovhb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vovgupkx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2womvywaj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2apzwbfsk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qvpbtufs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ntxrshos.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ppgfckye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ajrtpebz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xufjouab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vlczjvdu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ncgqlgjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2llmxxuob.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mpiuftps.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lqnhejvu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vxuqgnwn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2oxcnmagc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ryanczya.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jxtkchbt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xtiluexf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hrkeywqi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bmwjxefa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yawlikok.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fqxjajcz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ctqihdjg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2thgbikwb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xcrshtdt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wqazesft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lqtlaulg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gdygfejx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2djhgrkpt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xcxmfntq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yugdnouh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2aptvcrxj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qiosoono.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2guyggdax.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrysrgnr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2osgdcdkw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atenkboy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fjkhenhb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bfoyieao.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kjqhesaf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2foadtajy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wnacymme.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qehibovu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hlftufvl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yafsiqtb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ammexidw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bdbwueli.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xlujrboi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rmsmpvlb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cdtduzvh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ftexrrjr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzyhoqbl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ibsqdlff.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ozjdgfat.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sxdmgtcx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xedzpyqr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2whzzjydl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2albfcvch.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kuftkqoh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2krascxgz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ndcsufht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dvauphjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qjklswdl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ndaxqiyf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2anabasdf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2psmzccwj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dlzyduvy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2aunxdofz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ufqpdufz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dwcmisso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rakoghuo.html


<!-- 参考信息 -->