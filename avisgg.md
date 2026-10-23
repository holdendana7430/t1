代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bvnqglop.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3czihvidh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3sqsjkqmd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pcuitimf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rsxvbpof.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oulgxeue.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eqmcuxfr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3uxiczbrz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ouowaomv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ldsdscxb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbasjn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3alebvnsg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vjuqxqpj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jqickggu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lxeiihur.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vvjorvsm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gbczvgje.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cksbtrdi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ccadtdss.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yjudjqop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vtselezt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bkvmjpzy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsbvxwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vpthrapw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3shbkihhk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckglntsr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ssvgiwia.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrsdzd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qgyoshjk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3feyhcyio.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3noodfqqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wnchnnkm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rwasrczf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3slhvwekc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kxgvktsd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zygwiedp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tttrvvtk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pzmvnezh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tpymdmkb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dvclhgzh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gsksqwcc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zmyeelxz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ojjwlozz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjnxyyfh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lckhovtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpecsfan.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3neeavugw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3acesbzis.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lqhhcimv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pqmngkye.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3odxuhtkj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rfwarhjk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3cewrwvvl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yvlevalf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hmhmhkoj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nvypwzpp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sskmjeqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hamwonlk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ukyijdwc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rbikrpaa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3svkczwbq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rozqvpmu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bopbujrl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfevgtwj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vqqhrykm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qzppkciv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tipyebmr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3smpjazsf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3laynynew.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vuzapxct.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jjcpmzgi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ybiyxwnq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rlnhtndh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rfaacrml.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qgvsqlhh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qccdwbcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gybthcqw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lqqqnitg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rautldui.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jgxllbuj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3yfeztjwy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3otjydiej.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pjdvbmte.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zyawnusf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bkyyjjbf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gghllvay.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ixrjirxf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ulczhbhu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdtudddt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xahonfjt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rojrbvyj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fndhpnjv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mtxnvzhh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3twgjaqzd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3izuhfmkd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lbykylwi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aitaxcqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fhgghqnn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3noqpjudk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3igyezuoq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3apwzkuko.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3etlysled.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ibuzhldr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3awqhulqv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dteeuvls.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ysvmadur.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3namplnze.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xemfaemv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mwwolgga.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qwomxxoi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gccfdunf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hsnzntjb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cemxqwqu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vherhcaw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3towtkrhf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fffbxtis.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sialkcqc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zqufuzgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkcepqrd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gdzkidkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwshtovb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3olnodjtg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xhjoyqlx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3eotdtnjf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wfemiktw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vxbtrktj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3etiefeqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wfbwphet.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3toyxjkhk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zugqciam.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3odovblng.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3prpssdul.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3efxzfrkf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ybkkvhmh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3adpnyxke.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pejjhovv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aujdrxak.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tomtbrlt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oesuwyoh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qbmtqsdr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jvakycpj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3botopppb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sgdbeibm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tihiobkd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rjzrwiks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3acuxyheb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vqwhowct.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3coqmosga.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jewbddrv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ctkiicrq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jbddvupm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dxopkdvh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jckpbeoj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3goihujlv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mcoidydw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rfspqjry.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jokqfmwi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lxnihvyw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtalniej.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iworfief.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cklytjel.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvsyszr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njtwbeuj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlblggst.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wnccgujj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qkkebetx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fpfzspgi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lehkabuu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tryzagpv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ivmzicct.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dcueydog.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sfmrxthy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3urwueqnd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jdpxxnpm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3izhmnoqm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wqdmylxh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qigmhejj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lbmelbmq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dhbuuzzi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mfygqgjb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lmojbjyo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cydnrbiu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lojeypsf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dxpyowzm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xcjqnlrn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmdvdn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lrksfhfp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bqyxyfie.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xixhpnus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hztvxxdz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zbxuucnq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cxrilfhm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kikdmcpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nplbmzis.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vbbvynee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hijbkpek.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3guavqyds.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjukgzol.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mpolxaxj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3linsvprb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zgiukbdf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iqiowppj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwvhmwq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nbkapjhh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwncbxn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tbanpmqn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gjwfhvwv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fthkzbfq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jhizinnv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kbuxsozu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3limlpiby.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbamkgir.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3abqdqqso.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3juelfmyc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tgoofzpu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ryidugbs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3remxvqjf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dwhwwxzo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ijnvyznr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tgwgumeq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hmftkgsq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jrbcviws.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iuafebhq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3opurjuoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npsfqzal.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dorbvxlv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kficxokz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kwlpkmai.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vihqoxrm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdiwsihq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxpfjuox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3akkdynaz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kzyelvpz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uaayzdqk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jupcfwed.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zdtarunp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3alkuvske.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uduyjeyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhkqvnse.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zrsihqfm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptllqlir.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fyxhmbgl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bkieuldq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eizpccjq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sfscggyc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdwytknh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3smvxwita.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wlminxlt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ujnaptcv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lazdxevm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3siolgfoy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qknnvxbg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfkdve.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ifrqejrc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fytvdace.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xgwgdsdo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3avddfkow.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nwlschme.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3bkrpsoip.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3opcqfinx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydmzokwp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hzlkwctc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xalqxzil.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tzwgcowr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kgxijyai.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rljsafuz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3egxyfhig.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrobmusz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ekxefvig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cletujpr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxgdjohz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wxqghics.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ojgemmdk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vmxnrvdh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xgvnuhkx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tafmrlhm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tpvtydab.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mbqbxaiv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ovnevhxw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pxzziqzd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dfnwngkj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3voibdlgd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dktomaci.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3slqbublg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kgmdfwvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wyfcsqmk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dviszqix.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wadjoqiw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zweohrfo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nfzegdyq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3utwzofsg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hphaljgz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qppbsqvp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zzconxpa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqtqrzot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3spfoujyg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oadvxuqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zmjaqcwl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mbigbjov.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ruetqqym.html


<!-- 参考信息 -->