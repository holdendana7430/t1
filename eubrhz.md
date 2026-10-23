代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jjmbtmiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihyddezb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fmmytrzg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3msiovqgn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3deczyvcb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ellnokjy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nzcliudr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qdjixfus.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlwsldkm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xjqfmnle.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tvcnhwzh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnisntlw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zccsjumr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jmnsznxj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3cexfzuov.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3umptomwz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xteaoiaq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3enwrwazk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqxxofpi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3loqeyizr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xhqvgxei.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3impihbug.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3igfwivpd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xuokioin.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mdanmswf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ailkiprx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzlakxt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3gaojepgm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkmwhulm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnmjhfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qfxomgsn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nrwfrzqy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3viaabywt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fiyylhvj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kpglvffp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhfbmswu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fsvkczhg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tjzdhzny.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mrbtrpwq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rynianlq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cvcrauvj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgirzyz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hwxysazg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oddmwdil.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aidfdrrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xiowcuwa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hvrfyftq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vmhjmnvf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qngpnxcw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imfuemzj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hqczdael.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3waqfqyca.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsmjvam.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zgnoublc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3weoerfzq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3afnrfanr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vwbqcbya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rynsfvgb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3paoxcywr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mktrfaho.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xecgjgnl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tmqbgleu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dvyuqevx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rxixxoqn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mijlqdyo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3axjmjbjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nrjxmwvo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gkxvxxfl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3utiipmco.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nhmsjlwe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3duawqfzi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3iksbqqov.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jxmgguxy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fdfkegpz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3owzwolhw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vryjtjlv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3onezgjfj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gzsrwfhg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qqtggfmy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oyvzwcoh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qwheqolu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3psfpuwbu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3iqvoigwv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cojtkrrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbamiumr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kbnnjzpk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kqqfneak.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3brlepwtw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wgsaobcj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3swpjkiho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vntdkrhi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xjafyaao.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3booqvatg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wepnuqod.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fabrbnbo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xnfrymgx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bkeoqxov.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjcxilf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3icmolbde.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3whevdqhv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xiequlnj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qwdprtqw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yxodorjx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3igjghlfe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kbiszskz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vsonccby.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3twctxeje.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kwbbdfnt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iwbndneb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gxswuhci.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ukssicva.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xiatcxab.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hpnmmcah.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zqcghbmg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ndejghoj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dbsbyzjr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xwudpfwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3azqwuogk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syzuiisc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qjxgsqnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvoqcqex.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvludnqd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pgknivin.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ugsnfpdm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3juvbpixq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqqjtaj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dybhjbox.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xqsnwiov.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qiqhftbv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hrsaiung.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uvoqfzuq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wzxysxuu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hrejpmtz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hziiqvrm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xlzsoyda.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3midogcaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ojlltojz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3eexxbaqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nzkzjmfi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tbjdyaof.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xghzbihc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bojczdbb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgqvvr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3remuodkh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kftjulkj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3igjmdscq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wmajjmaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gpbzxsdv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3saglgenc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ebhqykdg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nrbslqys.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfdnntus.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xfcdfctl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rowsexfw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ljkscmhw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qfjgjtee.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3btfrrfqm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fuvwsvii.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oghjisul.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ubtbyvcv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdoijbd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ivjlvcat.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpwdmimf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3omatfbwb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcptiiei.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xyiobsjf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3twwvolkv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hdutskbo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3chmnbesg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3waipdawf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pklzfxob.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gwwrrgfs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xgeoqdgu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mxjdjzce.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nnwguvjb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pgctuacm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xuxlqqia.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hupvzeqp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hgpvmmqz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kbkgqbpi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiqdhfy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wzkfqqzp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3faszhygp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mgkzojon.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vznuhoqr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jsfvcwif.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qwrwbgks.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gjttptgf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jcshmbnz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sntullpc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3utemgfcc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zalbrrnu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dofzntsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpnymisv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uddyrhhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idvtvcum.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dkwlsacp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3odnhipgv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3itibjokc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rqzyutps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dgorcgsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jgudvann.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jfvpctsb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3edjcljuy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjkqvqdn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ehbgmzty.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nxllyvcd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wnjsbzhx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xjwlpbke.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sdqbgzel.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eghcjygz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3flebsufd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vosbhoyx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uogtosum.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3siculsja.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xvyyxmdj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wwmlfqty.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3duisccwh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tckecmnr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3txiqrreh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pmtiqsby.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3esyggxyt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3przbrgpb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sotpfguu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bdruqknz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbiuxwlo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jxnqvjgo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xvgwobhv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ywbipqlq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qpdvnnpq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yumyshky.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mubfzfdh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3roaxxosr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxiwrkz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pwxocvsl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhdieosp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3beainhxl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3htdyzjrt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aprglnem.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jorywwwl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyjkeove.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3agctafki.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xfehhlbu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kpvvwwgv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kiqhuwjs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwvtast.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3daczvwqe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qfanecsr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kozcypxf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ceozbbzk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ysldsbdb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rvxhwujj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uutfmate.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xglbdbmr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dyddtwdb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kfojebzn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nhynnnoj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kizafgxe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mgtyaeql.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vsoapbpo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnhovtqx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bjcemnvk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gjrkjxsy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3modlownz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ejjxiboz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxpaccmu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3bhznllyq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3affvqybo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3upbjvgtd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3khleqkjj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rhrfbnzl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lpyvlftn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fzrqbdet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3btbbtniq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gqmbrtwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3geauqsdc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3adgcsjpu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3trbuifzb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pkyevrgm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jbugycyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyoyzaqf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdesrzm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pfnwzqke.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nqyysyuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rcaeivyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsxehqvg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hupgjvlu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xspjgqyz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zwptkpht.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lqownlja.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fqjofvnl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljcdelyb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zexutyzn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rephfzer.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ukisvyyn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wnrxacgy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3autidwhq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hbeihzrl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dofqhuib.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jiumezjc.html


<!-- 参考信息 -->