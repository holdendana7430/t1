代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uijiplri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aynhwqym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lgkipvlc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3weeexdul.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blhlpzzu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ugkmmpgn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwkavbj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3obbmhtge.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sbgjbwuw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ujfyifxn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pinshwyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ueqxbiuh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zhycschx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zftlnuma.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3uavleezp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uytkzbnx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cshqzold.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zqahcijv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hojnszkf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3edtiscsi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ubnvvyxg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pxzattcv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wckspkcz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lgcdfsgq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ylelisht.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wfgetijv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3npllhegi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3porwlqyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgnnhyn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkhtuzl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gzaugrbx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hhxibcif.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3isfhpmox.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xtukgoty.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ufasdopi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ifrsfeey.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3snitzyqr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xefejkxv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3covapkwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqhsdval.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kxczfduw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doeqpzed.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xloxaloc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3diqarkwn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nxqlsavd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sqrvfpom.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ahyeolxh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pinxtomo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pooiqlrf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3tsvmdvoz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3daikupvj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lyfeaamc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ulkybfbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dtzffntg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uwnuakts.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rjirjbcp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rxndltzv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zrdvuwzy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ssguqown.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkctioul.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3txwdjkuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fumbesos.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uelfxjxd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ykdfsznk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xkaphtlq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3odjhqzby.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mndlzlrc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rrrsevmt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qwdytpgy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tpyirggn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ynrbokxc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bojbniif.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tezgxmxe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uzvbbavd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pjgyvfaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gyzvydtz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ltawwaud.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nehuultg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xymvenei.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wmeqrbip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdlcjvtu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tnwgwjsf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kcqpzngw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3uvosrora.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjgvxtnq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nwweyorh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3arhxdmkd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3haibkoqc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxkeuf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmiukjm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3badwckvd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wrroplqq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3oletwocf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3byzdfzcr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3czrbigyf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pelmokxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lyrzqite.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ziasvlin.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bplzupim.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vweyojjx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qfnploph.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyldgdp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dvqmllav.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jzefcxmj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3njrhvbcp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fookkksu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vrfrkzcn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sstgzibq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wocoxtqr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uifvxyph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fyqplzut.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tqhmagbk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3klfiwgrc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zehwtcuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sintldry.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pzfnkxzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bskpecak.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdavmkxg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yanhnqpj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ocrqnyvy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mqhqoczd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqszdzzb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3erdqdwms.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hnswpmjy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gzvlwteu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ibvvheue.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3keaoddsu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ehkdgybo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3arsznyad.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3caoqvmap.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tqxjgpsp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbjytevq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3elspdiku.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nlarcdaz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ybfpsiip.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xnvljfnz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qthkucje.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ovhyclmq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cocigrnx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3daffotrh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ukjdodcm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dtidshiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kfjzbjaa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zwuenqmn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3llxcycji.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lzbfgskr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3figdbqdm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ogvlifnk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yptwrxlu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wpsqdhpg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fqrfarzd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wzgwctqs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ckmkkefq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3opwbwrum.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nylxezvf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ynwoeifp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgbvdzp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuotpzgp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cihqiwhn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiufepbq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjivtwyg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mnltbfzg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xarhebzh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqrzwcn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ohsqgbtv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vkirkdyc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jnpdaapb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ycbnbeyc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3smimwnma.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nioysnhn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ooiaywdj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3joisqxze.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kitxsnso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vbzvtgju.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dwmnokzc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kalfpuoc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3pdcvpseb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3sqctscox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jaibvnkd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3csswmlin.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3iymhzyjk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qjwdcbjg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wabrbkne.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zigawwst.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ethjodra.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ujafzrqj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qcukofer.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fivafleb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hdzdhmar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cycvjuew.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ywocevgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnwynliu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oxkcnioc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pzqzzgvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cqmfuwyu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dpqodcbj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wgblqbqx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oimdshgh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgxcrvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xkuuqcdn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wflvkfay.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qyhhimyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hwfhxney.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gupcljbo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qxzacupi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsajuoi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rbqyzbhn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhvbdcjy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sgqfqcwg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rispyezq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hvunuxrm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3jvlzvtkq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bnfmccmm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uxlkmwaa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cksznkvf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mlxefmtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mbctsbwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hjwywpcn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fepequjd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rzqxvvvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzkazlav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nynjatzz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nhxihade.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hcayyfqg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnrdqbh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpbhshbh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yrzsavxc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdtpzwf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ehfovunj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zgivbliw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ippxsdtn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpeaqjmk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jxbkvhxj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bpvdpnyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3suzbkvgv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfchyuk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xsrualtk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gzngivbl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nhpdgozo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cmvtzgwz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ddrddubf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jfeizxtz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dizjmzfi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yxuhybdq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mdhzbjrw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mwbyknzh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ugunawpf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zlqelqtm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xqxzwecn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mufykjps.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dhsrfsov.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3furahezq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3njsasuoe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qrchcpvy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3txtmlwsk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gekgbwsm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpmewmjb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nbtjxzji.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vfpkwtvk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xgoysvhg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ffublxbh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3empzoqpt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tktresab.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xopkpmay.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pglvybjk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3snpnifli.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3etiznixl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ojignawb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bplcabbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rtxkvvpp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wxpyrcun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vjhieocy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yblffmpn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oikhprro.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dioudbgu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qihmkwye.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iqdocfxb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3edwynqhw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytizicni.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qjsufscp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xkdytevx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qqhehmdd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbjvtdln.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sdwcdnnv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mytmmvvy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fypsobwa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ivmrzjcj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhptzapo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jjxvsjmj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3envgisix.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rxtkkeha.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bixounuc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tnyzwnfa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wmlbewzf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3svgcoryo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3udskufcq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kudnhuse.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kwuouuld.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dhvlpoic.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fncesjuc.html


<!-- 参考信息 -->