代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ytjuikgn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dwcdzqym.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iqxswwjw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xpxatpzy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfodtkwq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twauebhf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2kselfeou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zoxqwljc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrgnbgm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jwzwsgvj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgvfnv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kqrinlwb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mvqpkwfy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2phglwuqg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqyodrtv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tquuecxz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aigfygsc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qksmjqkg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vsqkfrsb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jbxqekuj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzqfudyg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mvytrbds.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddgdxyrl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kohanmnh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2eqtbpwcz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ldcvwfkh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lpbmidbn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2oqjmknlw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ctuftrtb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ryqcrlno.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzukpifo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjnvudb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wxfnpomu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bicmcpnk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2miceflpq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xnruqmwg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2okiswnfz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ermskdwx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2amzcegcy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2fknknihk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2adxrquxs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvwdopk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oszhgshi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cijcelra.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mbsfsgjx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mfvfnlea.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dypsrzlb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkdkdseo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmmfpqgd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sukxqfrx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wcabnwdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ezdlyopx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2sxouwjqu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jvekuspg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sfxwvbyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypuedvfh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vfgofsiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcezkjgr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2erqwsgoy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jjxcjfbe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zxbfsngu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cglngfpr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xxcndsng.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hpdkgaat.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ntsxkfsl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gjvohoac.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2agzfjqfq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qbbowajr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wnelnohk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fmcitavf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2itqdcxrj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wzoasjju.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fseybfny.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gagazeqk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rjrwmasl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2deseawdu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ddstjomb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2utqwqvxv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fadorvkq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dtcvuzkg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pemobxhy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2onzhmtif.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yzwhoyeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2demboxlb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mmkrwnhe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zltpklhp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ljuiseko.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fymltfra.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ibgaddxp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gtjnqgyh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wjiiitkg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qsnlpfaz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2cluhbpvv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ghkvdsfh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ifsxesmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zxjmlewe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tgmgntrx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jdpkemyb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fizwevfc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2opymbehp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rbrzondd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2winohhwh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2decjxard.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fnbulcob.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bxqtyobx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2quqgztlr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lcjpbxna.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bvwfunac.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2grfmxvhd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fbszctej.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2edoayciq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qqfrcyou.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2goshszij.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2atqecife.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lbzqbkcb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zccrpwfl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ommicwrq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zyelbgdn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2skthjnvf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kqnylqwz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gmwffvjl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dhvvfjbd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rwvyvyfz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kyutuqxj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtugbhtv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kdlxdwvd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vjkyqcvt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tghccteo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hnkyktwz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ippqwcum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbpwmpwp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cnxixqbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sughqbdl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsxfyfpn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jjhazgkf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2liijprrc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2moycxhxp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2njxqrqof.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ouipofjr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ewiuumpa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kjkxrqti.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nxjlvopn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lrxavmnx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mfdgfgcz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hsoqodfa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nryqvutf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmbkphfm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zopleptw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vyyitrzv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ystlqpuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ntsuobni.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2unzlwmug.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lcmxsefz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lahhgdgs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lehoupmy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lbpuccwr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tzqxvgin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kcwcnpdq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ythkpqid.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zmjxlndr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ahafdgbe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2migfekkt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qqyhqlpy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ukkjeheo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ttteriql.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2quznzebx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zdczlnfk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2cfnzssxw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zwghklai.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2utocafxe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzqcrli.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jherwbcq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kuyobdqh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2acwvvgyb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrxpvmh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfkxdrhs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qtcapxzi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fwazsvkv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cszasqdh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2leqlqnvj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zzkvyfsc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hdkegvll.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ctzqlsdl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dszhuqdi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2amhtpard.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ixsofvat.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxxolgm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xvciqoya.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ybsmlmno.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2eqwizbze.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ovhoftoc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gvhujxsb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mlxkjkas.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ooxyclbl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mykqqroa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mespzfhj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kdhiegwt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kflxhdkp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2drnjwmti.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bbnvxmrz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2octkforj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2thjlyeqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rkyskqja.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2twhlcuin.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rvrrdocr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmlfghcr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zemahdbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksijobxy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2obiiyzcm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hnxwigbp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xalmknfe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2igquchck.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ezytxwdh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hculfcdz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oilfzwkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jxvngaww.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kjcutdtm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ewtjvddo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kzlqmfmh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lsinamra.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bzphyufz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2updqmxap.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rgijcnax.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgaocsny.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2poshtbzu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jvbgglnd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2crqjcbqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2szhgvocs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vuoquvmi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qazepcja.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bukislhg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vliilzxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pbyyaigj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eeykgxya.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2znphoffz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qpxfixjd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pblergij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hixoenyx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kozppsbf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wyrbxgot.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zwdtfdjs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2orkqbexo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcegchgk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2orqainjl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2trnykpqj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2siawqppj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfcmixm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eulrltsd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2blhhbbxn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2evzoxncj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gwkwvyox.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2etogxeus.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2spubjwqp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pgrcpimt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ctljbjbw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xormywuh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2blhmlcns.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2spscjskh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fajkpjtt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zsefxpvp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2naziwziq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qhvvsdev.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pptrozye.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kaitxubh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xbufqdfw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgpexwy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2caaypaul.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vxogkfnt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pcrgexld.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vvsquose.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fedztecy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hahunxrw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2iikfasmm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwydri.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ieevvejj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2smfoujiv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eonleuco.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kuvymjpz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jdrqffou.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dvhvbayb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wkshlkga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zbbigygi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvoigbjt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vyfkpuhw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hwftvfpo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tepzctnh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2achszwyj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wjemvanb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kubdyjux.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vmexvgum.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hdwxzthq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jsqnozaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bekaipdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hwagzcni.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hyjsqcfj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2evzueaui.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2snyokxcu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2azforbrc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iaslsokl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pxdzouww.html


<!-- 参考信息 -->