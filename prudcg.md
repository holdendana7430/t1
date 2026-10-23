代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ptyywuyl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3prurecps.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3owyzysro.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cndnfvew.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrrnllw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3autkzavu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hgxhrbkm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vtgyetex.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3etookbgd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zvgpvkav.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ptimvngv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmpqjaal.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ekblbrmy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hfpnnitn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uqnhqpou.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pehydmwf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hcsguzab.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3icosnkcj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gsecjbhj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ncfmbtpp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vkpuvyrs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3grrpvtsm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nlnctmui.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3trmmqlzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hhffyczy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3symccvkd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pmzoizpk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3pjnsdkvt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ovznolcz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqgkzgj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3psqfcskn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tkhvwgrp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxfwbeh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qdcobcgl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3djnxymog.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qgcbldsj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3iyvmuaix.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rvajskea.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jpuzxbag.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rvbkpxhp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pmtsgbal.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vfhaqpan.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yjzulbjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtfgttnx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gvvnbhfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvdvvbrh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gzmfokcv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3aggitvfs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fukwnlaz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lufbxbux.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3isvpixqr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zuqexngc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfbgayo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ejuxwgez.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wytovuwz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lspmrzzu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xiywjvyt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nclisqgp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qrzmdhkm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lscsgmbj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iojysqqp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yabbufru.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3udqiqbhu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ynaxrtnh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yfxnxfpi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wfshenpj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqweejlg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iatwvxuo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hpppekgj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jklybpuu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ejlcmhii.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yqooqubp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hxmuayya.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xxstcief.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bavhdruh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwmmkddu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3thxkxjta.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mtcixbuu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tjolycdp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ttzmurus.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3iojdliww.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uzdumxht.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3aawmkqcz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3teogoybh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhbkazub.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ghkrnktq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mgfihvfn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wfmyohaj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zqnudjjt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ccazdkmj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3noponuxo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ecpktanc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3puapzied.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kdwctqcr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ozlajhpk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ihiulbej.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bhtnafvd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3eoxhdbau.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zzrmtwob.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3orkqszqb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kijxzbiv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgugvoi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jtmqmmul.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3okyfmyjq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yfxvilaz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3byiobgxl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zjxolayi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3srfihgux.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lxjsmmpe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bjwmurlw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vpmmiwfb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3maenruxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3atvcddej.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vvhovfya.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3irbouuvb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3icuhpeof.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ofowwwry.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3geljeevs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibpivpli.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3cykhzsby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlgjbtmu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcpikooz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aiphzwsn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xmcmyqse.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zptsqmoa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffuvktkv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fatgfien.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3napunhgc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ccpmvhzo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kftyslce.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gtzqsmzv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bjiqqakf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3duyfdgwy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pwckggal.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3igjtchck.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lukiyhbv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lfrhpikq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ievnxqkl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3myeabovu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kntnnuix.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbzclpj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sdbwpmpc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cslsgzij.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hqepumqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3omuopllk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3borrltnq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gadcvmcg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ehxuvxnm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rhrkfwks.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jihlrssg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vmvwieqz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfgmitry.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhabvale.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tclmmbtc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nzwjqmtp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bkahtcxy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3quetpvhq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ecizpqbp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqeruhr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wagsyjso.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhfpvfr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovppgula.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3foekgefr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uedspaqv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmxorlnv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vtaiorki.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qlveefgq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qltmmqnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ptbqmoih.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bbprtjeb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ctgfszvi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cvhsiclh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zadnfnwb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rdvrrvau.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlnubln.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vupmtpcm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3etoncauz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rglppoww.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xgvbjqmr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lvoxtqep.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3piaswfvf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cxvjjpsb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lteljcvj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jnjchvql.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mkxocyhn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cfljxlye.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gubndave.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cjbkkvyq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rbwdgzsx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lktcxmgl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3exiizshv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mxjbhsge.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rzxizucz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmjgwmbn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sfxmhtzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbtpclre.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jobpojln.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrunutr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wksrhyjs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ndoyyhbm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqjwqqx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sphvrhzu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qspdxbus.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bamvbpyc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yyeejvly.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3clsxrats.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nyrhtjub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hxvsehvy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3orhtyoqi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qwihanbi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kmuojaah.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3okqsxccr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pbspjwth.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ddeavkxl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ecwseibt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hyqznacx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gqxzhzxb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mytayaim.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3baeuzwrc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3louirgwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lypnryit.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fepylsrw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3acziizmx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hxuyuadi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqneefex.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxciaqah.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3abuadwyt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xykpfcrw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kuhaidsz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xwussbrm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbnagph.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvipsvl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gvfgwwah.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xjnojlyc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqpqlogi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3isqskras.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcksgopo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nmjwtopi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovxtowjy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hfpradqj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3beazvadz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3asscijqc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wudrfbzz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yybomosb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hcgtwyhg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oiftvvcj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cuabdxqt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3peosgays.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zpsigdrx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3npxehvms.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3vkvzlgbg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ntvelvwk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3psexcrct.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jbdvzgpw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dwegdcmh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rewkczcu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3svtqyjdi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hnkeyajr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ladxbluu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dbrzfzsy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dllfzjhl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hcrkjntg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rxcvaamc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3csuegfql.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3brixbjjh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bftspmqv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yzjirvsj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdortkqr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uttkllly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xooqwaul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xcpwvyln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqlmnmgv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3oxbgrzwb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkliypic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qrwfwpgd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dmbbmvvo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jszpowrv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3chtvtqfn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3oewbzxtd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dptzhzyr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kvrapkzn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eidkjtwx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3osvfkrnm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xtopwhsw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrpcrjn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuziknud.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fevnncni.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ilxqdkcl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwlqtvay.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lxislscj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eeewybld.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3duiatska.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3igcgenon.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gyktobwd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmjnedhr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3atdtpwgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ynxtqojm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pbjoixqe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lcxyiqlk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3avctwfcz.html


<!-- 参考信息 -->