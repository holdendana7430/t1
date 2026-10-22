代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dgvmenlt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lkgnjzgh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kscgzlmo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ixzdbbwl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2trkkwraa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wojbysqg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2npwhqoum.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvhjfnun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ojorctep.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xajqyuus.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ynxgvyro.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bazoveyo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dmpmareq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jrgltitd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2yogepbof.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2klrobrnj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2azctyybj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2kezlpset.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aokorfjw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rbumhfbj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qhmabkax.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhbotenp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ucdwrpap.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lmoncell.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2seicedzi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pzvbfbun.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vloiaglp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xxmhrhur.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xmcozqxd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hiitfusl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xdbsihqa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fngfaxis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2chuwktlo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2auafrgzy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dfigrzdq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ujakxmno.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tpvctoly.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwpawqq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eipgaqnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvqrcvlw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pquvxmsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwgcqkju.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mrfallxd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ngsopyhw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2woqhnmsq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mcpkzjzv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gpccpoxq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yadshhkt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2twxeyagh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zkoctuvo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2tpbdoese.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bilixkrs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2onsfezdo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mptqnipz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nerwxkfb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jmilqmkk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ulcfcvno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2uogqirfd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zxtfnymt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2huwoolpr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wtexapnv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dgkuxxbz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2slvhjdvm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pbztgjmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rbmzrlck.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lkjeonqn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmztdrx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2waccuaib.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lknvgeqg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2edbeigmr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2krigjiuh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fszkihyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zevidyoi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yftksdwy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rpiaiqkw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ymoiootv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2uakvvqkz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ecannvaj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rpcuecvo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xazcfbru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sgrjnrwq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ajblzezg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dtcemtjd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ajtyvnvb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhsrbecf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mfwpspwx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgckcick.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2sutwbqni.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xvdigojs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lspijghz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hciqkyig.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2acsqnqvt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mqaumlmy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2npeenisi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2upfebvhl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tearkbyh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vnajxrmg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cyduslqz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2txqdrpbw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vyinraak.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eywepolx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pwlbhxtm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yskybitj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rgpzcsfj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eskmznrc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pceruxiy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fjlqpyki.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pefafcwb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oncbugej.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yvncvvpn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zefpefai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jnxgiaaf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zobcaisd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2erlurmbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvxiofer.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtthyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbcbhcbk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bmvokmbd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2diodebrc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2auncouzk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzfmvcb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2binbalhz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uxzpvfrk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xcspqmzp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bmscxwds.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2olqnhwzs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kfncqcoh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sjhhcaxy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2alyfkusm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dlbadtiz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tczeekwp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2efvmdyti.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xoorljqe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ppdtbcbc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2avisdeni.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qxojhxub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgbzcmu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2eyukowjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vhqgziej.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hqudzhwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2flfmbjkw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jepvurvc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kladrafd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tzywrzlj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2afotaoga.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qopildhh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wncztayf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdlcbvpc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yyvwknzw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tlojgvqz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ytcepnnh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qgfemarj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lheuduwh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lnucxkyp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvdtmgpj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2aamjrbbc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyoczvqk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kiclmchb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aubwgifv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qncxgpnh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kjnmfvud.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kvqptasr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iivccsmn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyogben.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2obaotich.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tdgixygq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ehlvbwlc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lpazwlgr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2doiavvtk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tgmdpyuj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmqbdly.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iphwumkb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xisrqcpw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2olweqvan.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ovpmynzj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cfdqxpmc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lxmvljbt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tfloeuuq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2trxtfctz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxkanhk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kqndkzow.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2uenirxcd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zmbqwtxr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ivozatvf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nqjnkyan.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2frjyssol.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vtrihdki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ojpffmsz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nzlzyfdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxfnldyr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hsxrdyzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkjdrtpr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2saysuaav.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jpxacvve.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vyeveztx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hrgstgeo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gcizxlxo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2noafsfkp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oawgllfo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ealwvrho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mbrbimbm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mvzvhooy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ghounzly.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lighrwmz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgsyjsl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ixkehicc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdvhcld.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbtheokx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qedssdbv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vhmmjfjk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xyliewdm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dtwdtpjp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hwahaoqp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jkwwarjf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ljjbuzfh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjwwxvem.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zutclgce.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2aabehhin.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qzoikefn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pyobfgek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wjtghmhy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yqlryhff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wsrjcdjf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jprcohsq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mobxyszq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xxdjkswm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqeyvqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zdolsvoy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ytcrkrwv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtnbavc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxuoxqkf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fvuibpiu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fthutbjr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2limrkqiw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wctrcypf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hclavkar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2omzazeya.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2egrflbcd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2werbdnbc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yojmpoth.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rzaaqajz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzanoula.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kczryvri.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tasfwiig.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hotvqxwj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iakwftdy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wmoagaac.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mmkdrciu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gpxkdiev.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kwdunbmj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lugbvtbg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2adsavqkd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ayulzzij.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ixpkdtic.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2szalzduk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nhqgsknq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbqwxqjy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pzalmfvx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jzetopky.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2msotcivf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2erppyorb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2azxmxvmx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zvmaotbj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dzerwbko.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqzcrtrg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2naafnjay.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bwxxzvjo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wioerfko.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nitmlsmj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lokrbgvq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zclmbnoq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wjkfnqzp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bjbgukqw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vlmnmhql.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2heowqubr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mufwrhew.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tidcjyuz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dhmlsyow.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhojldln.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fgpytous.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdpftlg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmeliakr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qajzizqo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fkpljozb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2beqbvpxm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mscteeph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ogvyznoj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2spritqul.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qbklhcec.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fbiffcyf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dgcwebnx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2leljpzum.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ftqyhqbw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lqwfewot.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2anotnokh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2plzximch.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cwcyxtev.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kgyhzmxq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxcovcog.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2orfvoylw.html


<!-- 参考信息 -->