代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2kbzcgcpx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dplutyxs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hppgtwfe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tpskbcqi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mzyaexxv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uclnbend.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ofszxera.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2neaimljm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhkcffr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kfialhfu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlnehyst.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hsipajiz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rttwohmb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ppsbkewg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2tjnqymlm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fnyjyplf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2oihaixms.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bvksxfdn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zifouwsr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hlfzglpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nzcdvven.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bumrndug.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yskdusse.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hjdlkjvi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hkcqwkqy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bywvrygs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fkgkvmck.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kwundpjx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iabwxdpp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gkwicjcr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqgudty.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhozzcu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvndypzw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqjjomm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jpfnzbah.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xpwpenxs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pgzqfxkv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jpzbnasf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jaibszwz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2sifjjjqj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pcgwslku.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prdpwbcc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uneccjoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hveotjtt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2facixhrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czhakbkn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gzlgostw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mejegmyf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vrvqpcng.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2giziguvi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dmthiock.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wgpagidl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ovepnhpc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nnrosggk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vxzzdjop.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zrzkvsxo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wseutbuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mzvwpges.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bjbtobxs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2spocvuma.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kjvogpdz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lohphmol.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lzbimtwt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lisfrnna.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dftimnry.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nfftfjkz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eprdhhpl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2emrchyga.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mfaqhhdy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tqklzinl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2smoqxzij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zmmzvhhm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bqfcagmm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2udabykce.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gcoxcmuk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ewelaieu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hoijmuyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2twgokyxs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zwesnpkh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wcsffcre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jwyqwhop.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2psdegeja.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dtihubij.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kjkasmix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2azhvinnm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fgqkzhwl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2aspsjgth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2webfrvxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sadyrkdl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lxkjkguf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2irrdpruy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jbalnggu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yrsgpbrf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2duudswbq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2azhekitd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjmnoj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yrpxwnii.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2frckpkjd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2czjqiwaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jrnjscqx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2puqzskac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ecbhcion.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tjgqlsni.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2chxyvmhf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2edqntfyt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wylsyhkd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2otqvofgx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yfvrvzaf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mkwevxgh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2erchlpuc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2brvyxryi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ynmtbogg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rvoomjzf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kbjchwhk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tgtnyqxr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xoiykwdm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2scznhwuo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ytnpltzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgbjiizz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ktfmvxzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfdhdtnn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yazgbczf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rmaietfk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xfkldcdf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmclegk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mmyfuesv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tumlbmer.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zisyszwn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wsodqdpp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vpjguoaj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2izdjcgch.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2unjjevcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gbdwiujs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dhgjotue.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vtcalqvm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pytxmzgb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vjrzuezs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xszltwnk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bdcjdoyh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ffueyxgh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rorliahl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sqhbwpid.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rvaqtcvl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nltouoib.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xxgqwkjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wtnzrmdy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pxrpksst.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2egqnojbr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrrsak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqmysamq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ncrdergt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnpjkstp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wgdcuvkd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pvshflft.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lyntxttc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zwqdtogm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxkyiw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ovrretng.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amhvpyex.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bekspoqy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gdtefpzx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpejbmm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ezdackyp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kudnpxyk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqeuisaq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rsaffoqt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kyopqbeg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vknquuta.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aanreapx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wtngvsiy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hkdyqpes.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cmcatitk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2owivqlie.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2iwelvrzw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2olonelnh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mdrhxvhe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xjtjjdse.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xxichxsn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uxtmjscs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ucvhvais.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fajhtckg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nsivgibg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gvxtpjpn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2imhhogvn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2baecqbgm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kcktxtib.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2npcvghli.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sewhwwml.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2niwncqmu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ispugcsc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dbmtlbgm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cjikxeyt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wzwdwpkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apnuthit.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gppusxoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekvuahjk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2whotviua.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdihwnwm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ywhksufm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lpynivfx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gzycjiza.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppyqbshr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2foolqbzx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mbmtxxar.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2onqnfpsk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rbddcejg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ryhdpfca.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zzazmrap.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2opqfztae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfbdbgg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2oqzckspk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2apscfddd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2elzmfmoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jnmdhyzn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hgsmqmye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hwzrpeck.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vmmztifs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pntuyyup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yarqkwtk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hhoxiknv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yefzokfb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rezxtuiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wuiovofa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ubplfxpz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkpfgrc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2auffsehk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2feehrcsc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aewfpvlt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcectlyd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2anhdsoig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hsdlmnxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ecygimqh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uqhemvnl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqynkj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tcbshnte.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2evtdplxb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqmreix.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ssfgetdt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ciumzmjw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ndqgpvpg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2okqirmvj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2holhtlme.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pfkyuzpj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hznqdljj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qvlptxsa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iorndlqk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gxxoitrs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nynusfyl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kckdwbro.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ltrdsvgt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xuxrklxp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lulyudey.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wcxnpjaj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ozhrixxw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2okboktgl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2emmqiywy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2atangkqp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gfvykmuy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kaddluha.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dkyctqca.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2csmpldqh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rgnhltip.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vjzrjqaz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2auctzycw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ielhqoon.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukvrpupg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xqhnvyij.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzltpejh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qwaeotss.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bsgyliqe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fumdarra.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jzzbnhyh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vawklmhk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpgzyyhd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ykjibskf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ofujtphl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2raaofpel.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bsqktftq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cqxlgtyk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qxnwvxuz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqpmeif.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgakfyi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xhpdssjn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zfbxijyf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yshlfxkk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rttzoqee.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ysjbkiia.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pxurgylg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ttenaoru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pbrbdkpb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rljbnmpy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yxlssxhu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cuykrqmd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hwkzrriy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2swxdumaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yulxvoun.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qkucnsjb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zbwjwzpl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fofqvzoi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rmznxeph.html


<!-- 参考信息 -->