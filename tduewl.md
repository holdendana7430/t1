代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bypdqozv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2unruufsi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vafozzbd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mtelcemz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vvjquoih.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2teavqcyg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pkwqnklj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pvgybqdj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxghaht.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kujazxqc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zzmsqwit.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkojasvu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2murfjapa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dqjrahkw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2alodxjfo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2slycyxdb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2csqsuqha.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bfxtamyg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2iggdwqza.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2glcpetox.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fysruekl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gdchktxp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wawfykpf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ofeardoi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dxlotiqy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cfdapbjw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tjjtfcba.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gtwktytp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rrjszkef.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rvmpgsnu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pkhzould.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkfcrgp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jajwzodf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fgaikzyn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2swlansvm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2asrtljws.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zntvahas.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hfihilwu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pkdovzzv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wtpkihwt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vjqqkbhj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmprhjyt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sugrykuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mogpylno.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hngwjezs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlqerspo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bijwnqsd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jsafoxyb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2pnahafap.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zpcwtikr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2phbdaynb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cubkahre.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xmizsajo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xqbtyfnc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2icdbgygr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jiqnwuhd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xerjhmev.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fabzmdfe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mzdowyka.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hwhssibc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gjbxoskk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2labvlbiy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xzlukorp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2urjvyyky.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2icofcapa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qvremmkz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eydswfqp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fzsqtqfi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hlnloflv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cfgfhkuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wachgyrf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qklrvxuk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hymqghbz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2axeppxju.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ntsllskf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2fcgadcct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ytsyvidq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gsyiujws.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qjwvupop.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ekayfbjh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qqjhdidn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2utdnuzgc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2twjwieww.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2twavalos.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kufudlxu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fdvhdlnx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dpgmjrko.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cuqhofxq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgsofaao.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mjijdcxa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wwxsuobn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lilwcuab.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kocieidu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2crxbcqmu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iszvaihd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2elfwmbts.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qiqivyyj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tyvirlpv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2iusjtyjt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2titazgaw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rsbyfcqf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ovvfijsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2clplextv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2svuxqupv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vbuvfyiv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2malnvgcl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bafgtmeq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cjarhxwe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gczuxlli.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ftdvxdva.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nvuyejhw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2geehpuhn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ccoathtg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nrxuxddt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bnjprfmo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dkwgjevy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mlstrfjl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jebuxvuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypdwabec.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bbcrzkug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyhgzbxa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rykjvgoo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lxskdafj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vdviucvk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cvmmdgqo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2alimkwaw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fsmrbsvf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vubzkjdf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2peutbnvl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ysmiaxhq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwzbhgat.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nxytsyxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oebssafz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zbubknnx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2oslnuago.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ldkvtlck.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vzecrvjm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2adyhipqg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jwzvuyww.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ykttypjd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmyfklj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2temwptej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npkuncou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2afzfnkjw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2uabrnhaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pqrfszhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2saavxxhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ehvrvtxp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2atvebzdw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlqmbufs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oteqksne.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lthadmlh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kyilxhhb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dlkppdrs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jajpexcx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sjlpmwwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jghvvzme.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2akdpblme.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2niyprdgw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wyngoqae.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iplpbwrr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsmbfsf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cxizhuyw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evcjxuej.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mwlopstm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fqdgabvi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qjjmvgdv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjmfoba.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bhlekkit.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mixcfnnv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xoncxzbq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iblpeval.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lbosvjex.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2trhypmeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bclysybp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kmjhdzvm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zruanzhc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dkjkhbos.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wjdvvqxq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hodffjwc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qycflgjm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2samnlhiz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xqwjhilg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjshesl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2urzfjowy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jmvwqmfv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mcnnujvz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2buhrebmm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hmglnxhf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xdplnnjv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ljyxpmme.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cnaainzm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fjocnkqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2solbkvqv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nwnsjrnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxjftxxp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mbbccgmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kmcjepmc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kkheqezk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqykhnd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fwuqheco.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvngcawa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nroozeyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2upcdnnkt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcyrefr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nfgdgjuh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pbdmwdwd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pgebhnhd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tjklpnkg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xouabgrd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2maxzrzcy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ostcdrnv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2exeqnwze.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2grddibwx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ahasopfb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gxaqwkrq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tyznymwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qkghspeu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2whcbrtef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ejkwwwir.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lsjybmvg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nzyiefsq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2efvywikg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vbxvmxff.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozikbcgc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnpteapr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xpjixkob.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wlrbhqui.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gonyseyg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ccjduyig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkohcyty.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyfyojof.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2avfwnelp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2arkdfkbl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2phsftrbo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvrxjusm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kippndxz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wqmlhfqe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2aicxuaxv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2iwwlvvvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdajqmcd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ivqpqyxs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mysyxatm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwolqsah.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2umqkybkl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rqcxvydj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qizkrpqm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vpbhcgrs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dezdtrwq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ngnibwdu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zfvyjbsq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2cswcpxbp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2aarrivjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yxmhhebp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2trypdjhc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2evymrgyy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2awspuzhj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qhtghrpu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2stpnryde.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tqrdmoqu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfampijt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2quisnusu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xayuecgw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rgwuscvo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2urdljtib.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cparfvuv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2sxnnghux.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sceovjyk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cgbazyzz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctfueozu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2htgjdrhx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2awmntpxi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2oeoztigv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mldixueq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fjzojrty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqhbmsor.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zxpmkhap.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2urzyizcy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ulqwcjvy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tsbsvsbj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hexdorbt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xjijyfgo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnusjywd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2eldfopoo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vsphtdcs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gshrsuqx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqsbcihe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nooclqxr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzaehciv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mcltvnze.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qombkvyw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eluokscr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2twfbhkqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cmmilkis.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ucglipey.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xbwjjorl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kcpobrfw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2npopecak.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2etzntwht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yuhcowbl.html


<!-- 参考信息 -->