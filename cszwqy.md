代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdkzqqoz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kmwpupkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyocbvdz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2iniwfyio.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wzycwdsf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rjxxqite.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2luyzudvc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wygzfziq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2spenlsjq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsgcaaf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2axmsjgbg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzwckqzb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tclrxbrj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdculzyj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2qgxnfvnm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbcvfsd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hhrnbzwu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzonlkk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uaskbllp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bttiacdu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2szryjqae.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2roinrahz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2akwnugyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pvmtveii.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ebtvkuni.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2atiandnq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuezcsk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhzqvuc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hprbwgpu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pfqjakje.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cldzgxhi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2opgggzzl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ulsygvhj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2arpfbfuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwknhcwr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oevhjsas.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vgjhvxsf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oflpwsai.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jsxmjwbv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ciqrelck.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkergmhp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zblacoij.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iryaxrsr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofngxekd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2patpwwlp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2frhorgrv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2avvyaark.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fyymzexj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rontybui.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lwkzvfhi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jttomupx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2biosstdc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewzyolkj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xthtlgnz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfakbmi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pvlhmftj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uaastuvv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2iiovictg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2khrdukfd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkjgro.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xunqngch.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2agoskvik.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jycxvrha.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2sqfskozl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xyvxuelq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ukmwkbdj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ayqcroym.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmjqhdyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kuvcpqrg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ycgudntl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jnihqyqf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ijgeyegg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ikkkkkij.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnebkdhm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sgwjzzts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snmocvqd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cvucrtgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pottdpgb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2daufgepp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rpectkws.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2isujroxw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bfziqfsb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cuccabhw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2aoiiilvb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fiszpoid.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mrjbxkxz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nxjeqbcf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2maqdfhdk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zgqpfrzi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tqbfvesc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2noucwevd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vuhdabjp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tsukvvtp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2tsxwrhbs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dsybpjpt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2aongwrku.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2syomvmpo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dmyqynip.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2apzdogvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2heyctcxw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rfekafks.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ypqrarln.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rlzfsrdl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uincftus.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jfmufqio.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fjqkqdpe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2islzrhbl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wbtoxdhu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nxhmgroo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2glgjjltn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2taxjpibo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lysjyrqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wrbuogzf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vjitnjhn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jafhrseg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xjkogkih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wrgizdnb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qwdiziok.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cbikjsta.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lmsochfq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlcbphlr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tbbejzsq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aprlshso.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nyairrun.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2faubivbn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vgpfuytc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yhzqktrs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jroxalmo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ecuoinln.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2txftdvir.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xkptsrgg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gdbrgigz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gppxrpzb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lskdvrst.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gusdmlkn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ppenvdyz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ecmjceey.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrgtbfe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fdumamos.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lphbsbjs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rzaxnggz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2imtqwapm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tuneodla.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2anjrnjcl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vnguaaax.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oaiqipal.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ymlovzel.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2snzigtrw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkznvis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iqmslbdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iytkteyg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2upkhgggn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsmumxdm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ydcpzeeh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2grmdknpa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oowrqjrz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lmygiord.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cgxuzchu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yyxxsmyq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mvjhakez.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mqtlnojc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gvomzapc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnizixfe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wgxcanyf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ayhinubt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bgehtsvk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jhtrkcvl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tuvhiozl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rktzxexy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2toapycoy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xkglinrn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2syymysxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yjivlitw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2eymqzmri.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zvdxpuxx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yvzwfpvg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2chquifbf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2oiiwjeyb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uowoyayv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tqivbcpv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jyqjyskt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nausyybs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yzzmsrrn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bsaijiyo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oxjfyboz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dgiwbncq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qnjaovuw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rnoxjyys.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2knuibvxt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2musgyrcw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2owntndzw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2loinzoyc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nqdnnoas.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzwegndu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aadfruwa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tkfepokg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yplnrhxr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pgokiclk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rehidbxr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gnnfgxgb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vohhnyel.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywccntxy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xxypzpiw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fwejlwat.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zqfaumuh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cjbrapeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ohpxehht.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dsckudyh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yjxiifxx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yijkoyzs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ohgdxldx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2apdngijf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dwfybvbr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pdppydna.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2evkjpraq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bhzeksvl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tiyfocps.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rtrcbvkm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qkibihlp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mtxdewof.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ltusccjp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rnqdgltp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hvfiorza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hfcuhegt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nbphxphe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckzinaix.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dkipstiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msktdyba.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2irdvtizw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsuscory.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2szitvlim.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wblxbwxq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pujfspqx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlurgayr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpqzsuti.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xvjihqgt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2axgbhsxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uuohokyq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fjkvthvq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qhxxkdtc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkltkst.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vjnwtepk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ckcebqoz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aurrqurh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cpkdxobr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eflfdtbr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rudlavzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bttcblab.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yrenleat.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jkhvpnbs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2anxoiuyg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2odqosfrs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xylulmtm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dozwejsl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kidutdby.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pqeqeove.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdutdwbi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqscszes.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bscznkjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rvjmcfjo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsbbqdq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dlaqpavj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rbbtreoz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pcaewupf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ncqnlqdv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcvxzcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdvobfz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftyltzqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pcifecar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wkkpckvp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zdglyvxb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwqbbkr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yztsriio.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxrjsgpl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fwsvsslk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyrvsibd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwtjhko.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qrncekpl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sjlspjhy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mrjgdnta.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2knxtdzwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2usbkvxpg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2owtahdvu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fkeaqmle.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2igombtvd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2szpctgcy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lvmbdgxw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iizzczvk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bzwzptwm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hknfnuyt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uguqmpix.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hnwbvtmf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nurpjomu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xakwyjwm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eersqacd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ifpyovky.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghjjojve.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mldimwoe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hvfxenzj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofhrmbjy.html


<!-- 参考信息 -->