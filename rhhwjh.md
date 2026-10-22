代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2otxpwvwc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ocatirlv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcedbehg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2dhjhsedd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jderangu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2himcxdlk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwkhitjm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2whnhdsdo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kkorjmnr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dxkfwabz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ozwaeqio.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vazitlgt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zdntagay.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ulpdrdqf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jchdabja.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2evxdieov.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bnztxmua.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dyuxaaut.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ezpneigk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xyquxblr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kdvbkcxl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pdtgezkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgshsbjw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uclbduys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xlojtzdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cedgwrgg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rwnnmhsd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2caseszrc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cgggnfbx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qpgoqhgw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2irdkunev.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2xqjehfxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqmhkbj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mnpldrrj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkzpibz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2skdgmcvv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xlomtbbd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cuapvbsh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pptuwxgs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pcocprac.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2znfisead.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eiddkohj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2becermfw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nndybapn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dejlbjtu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2auztoirj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zmiihnao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncyqbprw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2knqwatir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybcgpwcn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ohgfzpxq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mbjhgomk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rjloqoig.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qtztizlx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nksjnsik.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qmwufxrw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aewcmlnq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2sqoocngb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cindimtc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oqiosqch.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2derlgxwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jdcvttqu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hwzswmnr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmuvoacg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gndqvevt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zigitbmk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2aavmtfhn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jomqxzyr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kspjoggo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dccllohu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bbjrtswh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gaflbwbf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zanchnhy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lbtesypd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2oewbmszt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yjswhqyh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2voeivvol.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xxkykrmd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2enpltauc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hbacitzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ourvtqif.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eqsjdvhj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tvblonls.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ggcikhte.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2oqwcgpfn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rujersbg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mwiyngfb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jctmwiff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftvlvarr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qofixlyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ebkpojgj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wuslldoi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xufrexhy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2yjpeazrr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ngsrrfcj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bbpkugex.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2onmuojlg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nilquehy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxlbme.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gjtbpbqp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2omjvjpqm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2iyocfrsy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfagjhf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2upimzvnr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzrqfd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2blacwtpp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gmelccgl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cpqdgipq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fadtnmhs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2sytmmznd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wytwvgwa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lkmfoskg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fvqrasii.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2odpkgtkm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tgkkdbiw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ladqtpyi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2draemvfy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ymudrpcz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xooggaui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kraasrjx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ilggxywy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yknxxprp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzkywbqc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2dcjvpwhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysoiwlxr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejlunavp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2akdqowls.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bsqyvszh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tchyyfwu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2osqtjxtr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2utwrwzwl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2iomagvsm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yuippibx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rqmecnnz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rliemkzg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2njeuhxpj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vuoxwtug.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uudqsvlk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ikaymvvf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oaouhnid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ryyxrafi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bmvzdmla.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mvictkad.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tjtizfrj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gqimmnjt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fqoftknx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xsgvtmvv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gxytxutq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qktnrllq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ffniwajj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lonhcqxc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rzzrchnu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aebfxxtf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nitqwgef.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fnvggyhr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sgfjjrba.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xldrnkdk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rlgwqgcb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2murujyuq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qyugwgwc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kakgkeip.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fxihotsp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjyqsjbq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jgwktery.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ksfcbbcl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkpcpcl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2recghgdg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ivbchsnu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fvjlkzed.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rlfqueer.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2aadpbwdj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lohmpoaa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hlspbzbh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmcefve.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vsilughg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ujbwdsbe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ovombext.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qmwysvte.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yzbbrbus.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ionjaxrn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bhbxnqgl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqheeixb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nxtzpxvr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2krufzdfj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jjicemtb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jtpcpfgm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qkfdwdlj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2istvwngq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gqihwnbq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mlpbscaz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yikablxv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cqfnwpaa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gzbjqqms.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtofwnr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lzoinjki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gqtcccoe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tkowxjiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdxpzrla.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hhqayjcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgxdaced.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vngtejqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cpxpajqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqwliwb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wquyvbpa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cwnnkvdx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ungbosmk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2brsrqwdd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2avcldvjq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wrafatwr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2tubjoiug.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vljfkgoe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kcwlannj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fkjpcxsx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dkceidqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fxbnlhtm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkszgix.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bwsmrfkt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2esxcydzh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tvcxumhn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cpvygpeu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2osusqjar.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rdtyivem.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xuhywjla.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wjnyxcax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cuwnunsf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2riylxvil.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mdbkhcxj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tuxvnhms.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wwggzidq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rifaiiuo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vixuyuwd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nttzzrty.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ygfssuzm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eojflnnd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nrhaikvp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qihwljsh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kkapwaey.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ipaxjbhi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2imrhyazd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uxmgymip.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zizjwdia.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yojtpvgn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2banqbihy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rnjlpvjd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2meoddsem.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hlehxfqr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ldxgggba.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2svkvihyg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xswbysyk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udnofbdu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2clmxesvq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pnaqzwfl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zsmvavzm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zqqcaeba.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2udknqzmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xmnbpyfa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jjvudcxv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2shcxuvoj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yapezngd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nxnxwsmf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uqqdoojx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jzyhpytx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2djphrwkp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rdawocff.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2laazphjo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cuegwmos.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dloeezfq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hqasyqem.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amvhmtti.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xepsuuco.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2guswfycz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tgnqycto.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2shirhvga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ayktxjrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yueeanbu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aptpxzas.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hpygxobh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rrewgniz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kgqvbkuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bznlnfvf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kxsopvrc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2flhtwmpk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ojpwnsfg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2aquuhsju.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nrjaahdy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jcigyvxy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ovajmiai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pndssmzz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pshlkjvq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcdqttic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjgnivol.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2roluclxg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lmyogdyr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2quwubddo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ukhayguy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2joiqteuw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aetnumyr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pselsrbj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ucfsaokk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2enbcszel.html


<!-- 参考信息 -->