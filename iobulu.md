代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yajuurpy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dwputiot.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hysnflpj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtjeax.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlrdklr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dnhmjodk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ninhaeoh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hdnnogyq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2juvgfuot.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aamsuemr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txbgnhix.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qsskhwyi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkogqclf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2epnlmdla.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2marrwabg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2byeqnupn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2grzhvwhj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2prxvwdzt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qkqoqgut.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyukuab.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zdiukpkk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2shqwdzot.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxwsme.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tzbidyrz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwmciifq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ryrjhebq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wflxrkel.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lxtoenek.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vuiezglx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2upuwgtld.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xpytclpu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nszfqidd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gszqmnpl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qvjddlcp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ajnknint.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jzgdoxii.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2groaocdj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mksqnahe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ektlwiaf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xxsunpkx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vwgeftfs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gcyixdpi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oegxrhvi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ftkcujra.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kzrjugyj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xbtrnpbf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrfllav.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2soruuozg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcreqmc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwgocey.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2mwdaiccp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2afivukkz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtchjocd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jkjzhsbf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2achhehbb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2otjhdyip.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2eklnvrns.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jogupefx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fafwiwsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oceykjsq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrtlrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2riioyuiq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rkpfjgpf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kjlxcrpy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2almejtai.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gizhlvop.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sdhqluem.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jpilcnfg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbahbnx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hnzqzblp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bxsiubbw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nlncnusl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vzxeepub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hmuglbpd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fwcxksnu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eyyjyjxj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pwzcjrpx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lnwihmqp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2deaffqzm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wldatlob.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tjonkhvy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kvmpygki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vbylylzp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bcnmtvku.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cosiyuhw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xncshsxb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qymqduhu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tinkcfyd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nnwffulu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ctyyxufd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tdoxlguj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qkpvunjm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwunfxjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sjlxnmss.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eigregug.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2huhbsbmd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tgamlmrq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2skcffqpm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2grrzligd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2phuazgcu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2inpqfzih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2awbgmwsn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hrvultzq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qqfohpfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cperqwmp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2sqnlqmiu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhpsaguz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2irdtwxhu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rkqphzxu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kibiixfp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxbdcs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hnfaslhe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyqkbjt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2icyxkjmm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tnlvoytj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ubbhoplo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pzkrunoq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ngtawjqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2sywmrssp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rmwevqmc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xtxhqqoz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2crebtaxx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2djykcsas.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ojldwqzd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gwyvphgy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wxxdfsib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vnedcqfu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fcghliwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrxbiv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bxazotzp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2syktripx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2hkcwtxin.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2webgvpuq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2domiqyij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wntukqmv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2abearzbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpcffrbe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hhrbsyup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wlvxuntb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xquwabxe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nhqbzvvk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hwqmwlcc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hpwdahau.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vcguglap.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2voemxrgp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tchvfnmq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2npnbfptc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzrxskq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2srepiqhr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mqmndddd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kkbigvks.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bfdohnsj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2njfcyldh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sjiivzjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mzrtcrnz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dsipoapj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eovtrrvz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ymhlqzzo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ngppwfeu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tcobnvgr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jtrajmcv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ilctrvdz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dzkiievd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gmjasdva.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ejppgnki.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tinyrocb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tgswpkrb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rmndwwkx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dutysoua.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yginmunv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfmnthbx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zsynshlt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oewqhpvc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2anygpvnt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uhxerbcn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uowcpzgp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wwvoslvd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yusgiiuc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2braqdgxt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qdwqzumw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2iamumpmu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2rfkysiai.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fpmmzjym.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kagfmjif.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2otckodmh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vygzaanm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2arbywnyo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzwpck.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gibskvht.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kimzwwbn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rslizqis.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qbhwcfjf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ytcxobzu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vsgphvfo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sfrxtisi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2edyjdiqf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvxxuoi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xerzmwyz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2grrhyuqq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hytxhefp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ypsijozx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2osocdopk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hecjaugm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iufaadvh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fsgjpqpd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lvmbvmiq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wikhwtpg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gdrgsphi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hnogxqfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eddnltsr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bkgbybjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tocvjmgv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vzbhhtof.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hahgghvj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hqwdzglk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pjmxqeqz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wehegnml.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vlaxqiuy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhoonun.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2naeusrmi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bjwcqqbk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pdsgapoi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rvqiphdn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jpbilblj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sksabrkm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bicawlke.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aoahvdlr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oquzvjuh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2acexlatf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmqltlvm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ctcfdvfr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ulpslkju.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dwibosop.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jcdnilru.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oiwwwzlv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qohvxodj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sqhfhyqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jlbqbhts.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2iavaoqfi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2izxatjlg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wilerzax.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qwusbamq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iobrrrfe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qxhsuexh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cltixaax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hppeoaih.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qhwmfzxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aanzbaxm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ebakznrn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uchyvknt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sjqvnclz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qptxjsai.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mknvbkps.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tpwmdasx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iihqrlgn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dthggbww.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jllrxdhj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iztkdvnv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dlhvehsu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isqztlwy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cpprhxdi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxyucrif.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tnvdbqik.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uyearttb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qceutoap.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2svnwsszo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tvednvvl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hzwvtrso.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2imubkqbq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ontvqxvu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qrxlpmjl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vdhyrtwa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wpxmdfpt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wmltlxet.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fyhnebnf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jurfixnu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xojftech.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qlerudwe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vgiklxvi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jabxcibm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yddmauqp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2npzodnix.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rhbfvmjs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pakstptk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqluyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yychvhrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhvsldes.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjfitwjt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ctwgwozs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vhbmzfqf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vbiqmrfg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tstogayb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nzkiquyz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xezuppqs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2acbxqyfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2eynajapl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cdbtqvlr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ppbtioey.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbhhuqgv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2viblkfgx.html


<!-- 参考信息 -->