代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztkogjru.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2xrnqatqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcgytycg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2otnibuxw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dwvrcgtw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ilmzcdjd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufdxlnhi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnydyznp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqswbn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrjgwb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wuaeodqj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2fsajxtvx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2khxixoqi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbomdwt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sumbijgx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ppvsdzyh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dfnfemqh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsvawpu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iremxqjc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxmqmjr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrgnmvst.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mxmyxbbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnlcrbz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bqetgtks.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jglichba.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnxymkd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnmjalq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2svzttbns.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuddmvb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uuaoxfva.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wonjsmob.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kxtbpojk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2teidqjob.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qfuhegyh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sqntzvsy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2slmzzskg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2odoxmigb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kljcwgfd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zrpdhtcm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2efxgjuof.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ozishyvg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ndynmkfp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oowacqrt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ivuwfail.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ymftsohu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2unvwqtsc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qcuygajo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fzkzexjc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2dfezwunh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kbeeszeb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2toqgixhq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vouxqonh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tputnlxs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2frfijcjb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bbievkhg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2epjmttyp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ivorvvmb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fenyfetv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uflsgbeg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fqvelmen.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2efnkekfw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2umekjclm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qfmvlnmg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iozubfzx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2endrvnde.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrtadlg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tgeewahd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rigumuid.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mnlpovdf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aztrrswo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dwnrddgb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cchndvhw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wmsxlewt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vurzypnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2govbwdva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfhyoouc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2szhkxpmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbmdytlt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wmhaatvb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fcwqohpr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2oasrourt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2haiagfzo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ymcvdfjf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2noozxaob.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dmsfmnyd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wgcspqfd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zforqfot.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2noycbhzw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2aplhucoo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2aryfxajc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2salcwszh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sawcunhb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2stavflkk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cgjzabkj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rmpbokuu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xsisehjz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2oansrnrj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2aaqigdhl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pnlmiclu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ijvdpnyt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qtflxbqt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wbgnpybm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xgmplenp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ezkkosti.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kxjkflcp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2toecbjus.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ngftyuty.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jbdigvhl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uylvwlwt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cmqmnsqw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eqswlory.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xasuriqe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqzfpko.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mltcuptn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2megqueek.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dzvuzwhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xqhmgbdi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2btqhtywv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ypphzhfu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ydnofedf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qwntgepc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mvgqkvok.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2olzyvwbb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bjjawwmj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzhhbcdu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ewymujfn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mwyfowgr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ufzfdttf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfirlda.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bfirbzpc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mnofaomw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hkqxycqr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ubpnfuzr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sjmbloza.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ywcnfusj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2focrxary.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sdbicvld.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qnkkguif.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2izsjyphl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jnrmjjpi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lrostnbc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rhotocvg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gmjotucj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hpaweesx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2awwlweyo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ewyahpbf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xjegwyun.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rzcvmspm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqffydo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2huyhcrzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scnnyaqc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bikyrtdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svzmhwiq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2arykfuag.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2diccqvfl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2riiihinj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2umkuplbh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpiefiay.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nebirvqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zlyjqlzb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2sufhitun.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aiyhlsvq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lzfjoyfe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nzyzgyvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwvxazw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ksbptrqe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jimagwfp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qaiuzsvg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pupznihr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kqufwthm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mwjtefuf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2neczjpzc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nhnccoxz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uvzxmlic.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mjkljsix.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ctklphzb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kjqxgqcg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gdacnedi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lymdzevu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lhqrkvnq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ngvqdzwb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ckigvvvv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rghhembb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ehepwsnl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2okhdqnzu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fbiglaog.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pqeqglts.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xfgfccjg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2avbenvbx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xdhlgnzg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dgtzjeub.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lhzqzltj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edjjcpyy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zufcehxa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfrqkro.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wofhtutb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekelrahc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ilbtscig.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2adeqzqnl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bokdtmoa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tzcqkqvz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yexuheeb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cmhhwlwu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jdatjomz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sgsitagv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2iwcurojp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qotnleoq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2apetcxch.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ufsbquby.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fgpoiqdf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2awcvtzvl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cvwdselz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qgsqivng.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rzufxmfm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mnsxsmkt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gagaktsp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nupurrdu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ppmhpyna.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dssrpltn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pwabfznj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rsccyicy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nfspgvfp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qgiaxkeu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yswtxupl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yfvybxkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bffmkrkx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hqffcwml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqbmfshm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zmtmywak.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uljmzaqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bzcbdten.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wxsnhurr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ogpoymdp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucayduxq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2olpxmbwj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mcxwhbgz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bktevfcq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lvpkwmoc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ltvhozup.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ngorjgso.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkacfur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgwvkmn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2arqbaxcw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhjjsgou.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kmvpjnwx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rpwhmuyj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tbczprnm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2klumftxg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2viulibtb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gnohyrrq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nqacwkrz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rvgkwlez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iencjhpx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xgyubvnu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2koyktwxo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sjcbymoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uonegrtl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lgocrngi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2asvvliep.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zgfvlnwp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xydaxzbu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2geskhqwa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibpxooxo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vlnjlvdm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2esrcnjpf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dpsukkzn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2krthgzml.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtiounhx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kifnbtyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pfqtklft.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xueioqju.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmhqxvnh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzbntkzu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptnuahiz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vsdosawd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohkchrvj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tnjnspti.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vjzrqcdi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xbayhuzw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2abatrjpw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yjfachfe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cusdwvqu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xoxquymu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rtnlnayt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2suewihcy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vyveffxd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vmdshqoe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ksxdcvns.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hihaytdi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yrvhsvtx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ydatfoqa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kaczwtyg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdtpapmw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2upeybhhv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iwwokrgq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abeqtphe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yimjquol.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zomtszrl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2swzzmnqz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2falpxeta.html


<!-- 参考信息 -->