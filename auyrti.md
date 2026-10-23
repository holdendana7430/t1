代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3oxcpefjw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pxnsuvsf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3esbbrnig.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yonxulhn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlxmcxs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lblkdeiw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3faszfjxw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zingmfml.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ophqgszc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3jpboeifv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcqqzvsw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkepwzk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3lyipxxuh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdthod.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lwzrxvah.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uynsjkcv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xvomimen.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cltstbut.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqrjabvh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mihngvch.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3edryvpzw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dfpidhfi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yqtktsah.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mkxevvuh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uagqkoua.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gozoslfi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nqzaahfx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3roxyknmx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3paepeawo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3thgodvyf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lodvkkew.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wyhoivoh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tiayiyib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fbpgelxs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hzirbnjq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdickox.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obodimkd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cniceznh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ksxkmjsb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bnepskea.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3luwgxdpp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uqwsmxou.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3khadakfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgccixoe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3seygxqqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrhuzmuu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3polbmyii.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rztncuow.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tpsxpuqm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rlsoqqvy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hpcpobwm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvsith.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rusaopee.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xrbtnshw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mgsyfsjh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jkbihjka.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3torznhkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jkhoypsv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cdqrjonu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ttxjnytp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ezuzsknw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pxxyuksc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pldtoflb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uybadrho.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zsdwpeec.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ufutmpcr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cmoyhzzz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hysdsypj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3heeguxdz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwgzbaa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kuiyjjww.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oxcxvxug.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3utehzmbf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ewqlfaog.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vfsrxbsm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wccnugww.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pmobimvr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ywbcrffm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hpwiftuq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rvwovlwz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3kkygtuxd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ortfwllv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jlgpscrg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3slhrvewf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgksvwly.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wrhspkgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cfwxwyli.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lvwaqdht.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dhdvsslp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nblhpasy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spryicst.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ewafgsbn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yzykvase.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aiqzpwwr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqelzg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ikphaydz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxfezrc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3guovwgxd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpqwsts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gevkswdo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vxhtxnqo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vmsgbbdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uwdevpqx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pvugclbb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kzltyhzh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cvnixoba.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sjyokvzn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3plxaiish.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bdbyiwou.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yqwenszs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3plnehghj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hvlzogdb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pkjqwvkn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uuzyvhms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kzeqdkgm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gffulhnt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ghqkadtz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3grmuvtfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oorxfiwj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mmmqftrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irwzjtry.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjhyotdv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3expzjrhu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rxpxwixx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hvhfuevf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jsbipsrh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3anczqfwd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pcrbftub.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jklxfvqu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bpivjudc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3igpqybxz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3enrtgfin.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rzfadrfk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ishidyws.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fsyoywzn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3huqknybn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dufyscwf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wgmqtjmj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wwrhctmn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mnulrvob.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bayvuxyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tbqtzixj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3subtllbp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cptspwcr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nhxbdcrd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gbinbxzb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wyfonjxl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3caoyliju.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3smvwlaxn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wpqgfyzi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ertmshwb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bnvegntf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zrehfdtd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3emrkgikk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wevaofnp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jhyfmpbb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yhqtddcx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ibkidvcj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmuubc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3osnkowos.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rehmyhho.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fimzecwr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktvdprxz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tzbxyman.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gvhdxahw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xczzlhwo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3uzpglwss.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rckeiaxf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hxhlkubu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3irxofsbn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmjgoon.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pdihdajn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rtnepbyy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3belipjiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3akzbuled.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jekmqpye.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tkhmxflv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zshahvce.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mrqbqmvu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bntpgbuh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sooqdsfj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3eyqbefpk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nmcmupnc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hkafcjrf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3erflvawa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3eoxfygzp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3yyyapwba.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dficovef.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ndnckhnj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dbdtycix.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3iwuwxhdg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tgzaczhu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3evaiffoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgqwtbsj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vyhqjksf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iviwhnog.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3snftdqkw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jigdeygc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qvxzrpwj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3olyrjjud.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bcbwosqd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcgpzzx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zwteiqhs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwmtga.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3exsxwvjd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mhwpxibv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3apbfiqjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oxtmumlf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qomwlgcu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjftkbya.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dopihozp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmzosryi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gvkzmiii.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iffldswc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xjerarvg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mqruskye.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uhdpidan.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gldnckqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bceqbggi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ldjxscfy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xjoowwks.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ayjslxah.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3crrphohc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fflpwccf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlxqtmwu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkfpyhgm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3svxkgbkb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkbfsecs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3khzkbzsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mtnvtekq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nixgdudi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qjuqiotd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ewwehmiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghthyrsu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xddjyetx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpovuvkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3arxxwqzu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ixvqvjyp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qpirfcxk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lccqdsfw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3irepckcq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqttwbwm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3grhzzsnc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdxiezev.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nzagpnjn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3idtaacwc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3czufeqjs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ntkzjfll.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ceyjhwmi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ndjzbxhq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bcghuocx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fwfonppz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ozdgxqdq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3decpoxcw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lxvqfzie.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kuqwxxxl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kkxehfoa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gcdfvfny.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mtawysjy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tgflgmhh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjutmtm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nuureuht.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrunxnvs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3utdgfuke.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lsoxroea.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3llzlwgmt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rmtimblv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fleqpocs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3inhybqep.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wzlkjdwl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pllohxxd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3txcedwiw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3okesmyzb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dnopnnmx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fxylkspw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vtzrwzum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3shswasng.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vjmabexe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hfvzeqcs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3eonukswg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3chzcyjdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qmclmipp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gstehfzt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wxsiaemn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wzlohxcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsmsrmph.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvjsldwf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qmjjevbr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3blhnaxft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bayohhlb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ewfqilpm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qqnaveop.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kumuydwl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fnaqrmje.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmzummfk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ctlfdgfh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zwbghnku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eumvzrau.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mzycvifv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lbgvwmhk.html


<!-- 参考信息 -->