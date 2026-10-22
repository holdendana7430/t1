代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fzphoasm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hxkgeyrq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwbsuuie.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jvsbzndx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vtwfktcx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2sgckssqj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mtiyocbh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2osmgbrpd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pdvkxepb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pqoqguzo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wiqgader.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jozzzyhm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2lmfitjqo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ccrscced.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftzjpbsp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mhbghuck.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2stiqfyof.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rmqdbwhj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mdupzmws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ngfxelnk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gyoboarh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cvthwuzn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlracle.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hfloagee.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2asbvjikj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyivxdc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmxoxrrs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mygskrgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyjnnru.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrrdlgj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kejhpkga.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mebweviu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oapncxzs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zsuvltdm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nrpwngjs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2guhvtkdp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gvpksrfc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ougzsovg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cdnbnnnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqhreyrb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ezyiqsay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnupxzvt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ameuurdc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xjeqxhlj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bfgraxni.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uxqekpqs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cylcfqqj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cxercyih.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2jlfbcoqj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lolyntza.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lwsdjwzg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ccmrowcd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pqeobogp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xzvidtyd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zfcvhzop.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fhjemlbj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zijujxfc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jwlkmfwm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ylxpgpar.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ikiozvec.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uqnudupx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zidpecpz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2avfacjio.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fwfjrsve.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kqpquilk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vzzfbsbc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xyesfite.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qpijtyde.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xanpeslq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zimvhkvs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2maenruxb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nlonzwuc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kdkxjyjq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ntscusgc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wlyadllt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yqmhrlbn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ycpnczoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jaicrice.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2fgljilxt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ihgpckez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydiufczy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qyejvhzx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lyedkrmd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hmmrojah.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2irnugizw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2imxlefje.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pckruutk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kwacxocx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qtjzbpzb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cbpbwrqr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oomxdwxt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rtvbuynv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfsufdw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2afcjvrmg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2msedozwn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dkbalifs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2whxxcddi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2whsipajj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2konqmnzf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hekrjeow.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2grnegwxh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2btdlefky.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iildhqev.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iprpzafq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kbouflmn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2taulenpp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zxvhazoo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bknrfxhh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ysbvlbgw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hltqpfoz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lxiohyuf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ixqwiuzv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2esuhquwt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ofhvuqjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2equkokjf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2oyxpbtet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooqrsuby.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ixkurppe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zwbfvvdt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lmdvnbln.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfxzrnm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ndqkvbgg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sfbfmsaf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hbdzhpjm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wtohadng.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xqhlvjzr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2btidzsad.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nawfpysa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sfcbxcpf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ftwkyjxp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jxsazige.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ucmsvivm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zjhqhyxj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2roissirs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tyjkwpbl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wvnykahm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdkwkou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yitgrwxr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mywhqciv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rqzcnyuk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2euluwvko.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2csxdngzm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mydzsxfy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ahmjafcs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lajpufoe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnsremuh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tovpddhm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eepjsodn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aqvwpchr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bnntkjrc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xpphfejf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2smazosti.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mseuwrqa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xtwrnzer.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wmzxumnz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ooooinuh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jhmnxrdg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuunncn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxqupgxp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qtwinbvy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mbnczjof.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wmtpvlak.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vuxreyah.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hykkmjpe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jvifiwzm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdwzjfxc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tvbhgvsh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qyfhglfa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ccqijgvc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tanusdhr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ypczepcr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qdrklgnq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2udbadcff.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yictpccz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2frhqnynq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ziqkuxtz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kdzidxtk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2osrgvsml.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2swobaqaa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zjmodcnm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ksemgnms.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qmtjezxb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bbvouuaw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fsrkulea.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2obcganaz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ocuzyrsm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wezqxcpi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2aviatoar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zhgphjyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2verwthyb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2chkjbmod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqpzhtjd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zmwjnwtc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cilckbij.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ucoifhmg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pgshlzka.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2taaisuwd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cacsnpre.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hkcmpozo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tlldjuso.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yvusnzzi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gkxobkgi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vdvhafax.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wbxynykq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nplnwxyg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlwphwmc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xxxnwzpc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efbxojho.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vezxiaea.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vpjsfqwj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rrquqsoj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nmhnbwdb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ulfiutnu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nuwlgmeh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pfsvwuvo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eycevswa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2actaxcju.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2odldjvwb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nfjhjjhb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qsoyazyy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnpzupz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxitazqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jffdwesq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2swqhrmdh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2blpdukqb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yyolbipx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2brprpmsa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cllnzdny.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lqftqyoq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuktekcd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdntdxz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vulhlgww.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vcdphcct.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fapzansr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2sjzvxzsp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fjsrbcmx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wapvqvni.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkxkcwem.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nzlojfny.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2obdgmkgj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xykpnlja.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ozmcgvwq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2asvviwkq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhbehvdb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uvhjbans.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2stvdbyuu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gtzrzeid.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2seijfavy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2moiauvfd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oglwymer.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mxergkai.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dmhtrvut.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2culmhmbi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wvbxyuui.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ebcjjwlm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yibtzwfv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2obsnbkrh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2crcylfjz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fuxitpez.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owrmjmmh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvslyihg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtfiuvrh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2npkxaxox.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qtpxonlu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gmvuibvb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkfgqvlp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jqnxvyug.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uiqhklfi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wovknrkn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2icdruyqk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cgntfedd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ldljtfrr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hfrebaku.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kcoivxtm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wnzfntic.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuftddux.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fqgzqpeb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pkfkiwlr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qftxywqz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pkdrgoxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2byvoazsq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylkzcwkm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cibvpzcl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2svsxvzxf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iqymvmmd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zjlbjdhc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uyabctwi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aehbfxas.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xmamvdss.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2npwsbgbk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwuwyvcm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2frfstgpn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gsvorvuf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gcoipxng.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2npvmjbda.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jlkxujlz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fqfujaql.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tzrzhizm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2thxywowx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tpjsoqmi.html


<!-- 参考信息 -->