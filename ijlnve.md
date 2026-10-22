代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2aaxbjuzy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2blvykkvn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2niutgrvf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rmuufayf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2njtzsopo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbvvykbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmtgwpee.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dnqsagwy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbwtzib.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fdqckypy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yciaenqy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sihadxzz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jbioopsk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2euwbycqj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wzftaweo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ywmuwmbu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ioleeczn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jdsbstiq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lmtrjuib.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ovaucfdp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2msoaogry.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ulzjtxqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ubwuzuqb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvwzlw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kpbtrjwi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rcplbrpa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bjxfljes.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ppdadjni.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ojterxqj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fussupen.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ykxjcxeq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uhcbkjrv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kjnaiabd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aclnsqpv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2sdtdvltb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjramlr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sgfjitla.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hgroizdk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2toqesjts.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ufkdtqpz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2efrukerr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aiweoiha.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rssgjrdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ontxhnsb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cqgnrpzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbdcbyjs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fhheyglf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2spuekmcj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2swiqiadq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ikbxpywv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vijqdnue.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vfrqyrem.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2usggnady.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2iitygqct.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hiaeeipl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fkjalzkl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pwjahcjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2iukbqrel.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2igecltnk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wzmldkcu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uvhrsjvv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dckbpwbs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2txceezuv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zfduhndn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qjnhvtmb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2kpzcydyr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uyskkmhe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mdgaxykf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wkfgamer.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2czzxoguv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bobhjljv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pnadbvyq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wnynsavm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gdanhzrd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wftjqdjj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jnfvbqsz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2doedefah.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ykphiuza.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2eaaekybl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fyyrtrqt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xnuvicgz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gwrzhgoy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wfulbvsn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kcdysrcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nddtdhou.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ejjkpvtj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rndsqvgo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dmhsnztq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fkferknv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lhoizgqa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnznnega.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xekjkilz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jtdenpmt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jiifutew.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yuujsyls.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yinnlakp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwjehxm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lqncxomu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mkaqtqtc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kavdeeqk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2homwvbvl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kcfajwww.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qpiemalr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2foqhnrmq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aekgevlb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cyclcknf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2clloxumx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gucemhry.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mneqncok.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2lkqigvci.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pvxvwcqr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ulwnqsec.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2swqzvazu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dinpizbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gtxsskct.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bmcxieny.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wcbywffd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2omnzfoeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thduicfn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cwzfzmgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmnaavuq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zpjonmfu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mfwkbpge.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kghzqarg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mjchczby.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tzdiqtna.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kfnselck.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jejxygae.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rhlxfueb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dtctikoo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2obvtrfef.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2akblibgz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zphbxaqt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ffimhxlj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bdntpksn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2izsvwmzu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pkdivbgf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gqaisuqu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gygetbsq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2oscvwmzv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wavkkrjo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wgcbpzlw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xatyxdqu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zecehsff.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bzycjxoj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wnoihlrx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2whryisoy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sdycsrru.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2srvwyhtr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iotlwzcb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vlkkehih.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ruuvufgi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mqhtqqua.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2goubokze.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qscbrvjn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hwzorcjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qhvcefwu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gcqskuai.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chvsssdd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxyzlwh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwmssau.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bsklfvci.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jksnljne.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prdzkucu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2btmtiohz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kciaewam.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vcwplkqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcnhlbip.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hxbklszg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lpzygjiy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bqvsfyuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xednodwm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2enqqoxbi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ytjwyscd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dxykteba.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2coetmfzd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zmuodzcw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mqsvvqjt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hnvapgmt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xhuwdrns.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zchaeakp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vpydbjpe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bfizpkge.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yncpmwlg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rlndiaot.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fazjxzhk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2acaxurqz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rdhvunon.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xeepaswc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ydaxklog.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jbrsvcro.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qnwbmgwx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dofiipbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgxmnnar.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hzccclzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdlarmhg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kguqpeoi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxweeggp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tvcchmqf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jnmhrzvz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxhjune.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqidrfmm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ziixrlil.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tokxfzle.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlorhng.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bsmqpedh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jblytclr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnfosunl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tivzzvtg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yangntxb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zffrwgcz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfgoiuqr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xeukibua.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tdkavqnc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xqhexrgy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vrnmcisa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qetolpxx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ojbutqas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xvujdbfx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bajolulx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gengjdts.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2skszylyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2khxtcgfb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vslztyoh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2funzjsik.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kggzemdc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rczisrmz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xsluuyeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2amcesikp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bkyploic.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjbbjox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2maufibaf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mpdmlxyi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwtfkta.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nccakrsh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftwpwdux.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qzreqqgh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rlubyjyv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ruuhyqxz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwxtbhz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2oglzzzji.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrbibgfn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vqjspabx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2foaxpmso.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kdibopor.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wqlgedbp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2musarxrf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ucjhisbl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aojixyof.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2evmrukuy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2swjxaqvl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mztktqia.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nuhfajui.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kmwwmlmk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2yrajelnu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ioljejav.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ctylrjqp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tizvddym.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bhwxwmrx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mcedsbrz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jijpvrzx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xrgarchx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2legretgq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mmqcimvi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2htnouurz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gsgzyrya.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jksyersc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pnkneelf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2csjderiq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sojezyyj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ikmniugd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cexgqlvd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mjvxjdyx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cigdpdyq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rhbpmjqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2anakytda.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2blhhkoxu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zwcoxbjx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xzhfnsip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kryfiaau.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uvbcstgw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2exdvfydr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qkcuvbsp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kqdvrglc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2quxpvlxg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jresowbs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2slborszy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qkqjxgzn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dlhbmyvv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mejbrdzq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mbybdzqv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rmmaawyc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jpjsnodq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2upqmawjn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rzmeuksu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ltnjemoj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wafdebrj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wxuuimqm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wjjkeigy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wdqsxwzl.html


<!-- 参考信息 -->