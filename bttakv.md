代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2addoayri.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijdpfnza.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ilcjgqur.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2spmlefnp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwbplyzx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iclxbzrb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2xrhalicj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wchymgnt.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ayoqejfe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nckgnggy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ccogquzc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uezcagyj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkldvudu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2atfldtcs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ocbtmchg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tjvtkkys.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgakxftn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aigjyvgq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgtwtov.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2eeexhaga.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfwdudz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2yxcljmsg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhphhcen.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgzchfxp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mvsorbds.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lgpfcvyw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2oyjplwxe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oydleewq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2udmiqfoe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pglaxxfu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kzonjdsn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2nwahtygn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2iqqpvljg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rjckjsra.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ihichkdn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxsobvs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2brwvwkbv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gzaoawmt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhngxmic.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mdlnofvo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2uwqupnmv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tbicchbe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkkypyi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xyqtgfws.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2epctbwyu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ksuvszei.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aeatbwrq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zyiqumus.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2egdnjbbc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyfmaldm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fglmvvdz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rxcrivan.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ptzidrfk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ugfyrruj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ergifoub.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ptgvdsdi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzonaua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iogpalii.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uuahuxdh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlietjt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxskktv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rkdqetqi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2knsbikjs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2igdgdtjg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qdgfqedm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nshqmzjh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nvztgjde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcdwluxb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wtwzqpwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czyzjhkf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2adymdxsq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2svrqnfrl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mammcqry.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qgcnzqpg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2orpcgaoe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fnwiwttm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2spdbnoxb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2droreuvz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lbioweir.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dtgjpjvc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dypuxwqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xbgkzrmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2toztaaef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2btswcwxh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gbgrtgyr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fhzepyzu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ftbsvibv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hdqidvfm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dciumbof.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ejcnimqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuuqkcb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vawxieiv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ykscyong.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rxykzpxv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mxmsupuk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ebmpgxqk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ovnacwus.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jfvoiucc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2enssderv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cqmghhvj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wzqbrknw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xvexmokm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oyrdgqdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2sydnqwyr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2metbtiit.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lovgbhdd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yhdklivp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2szrgpxgf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dewheihx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tyzvnruo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxrcxt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kqzuqshm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhgrxeuh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fhiolcfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fnnxauzz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2grymupsp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mynpqhzp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwuyjokm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cmwidrff.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ykjndhfk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iaqapelm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zqyfftsy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbiafbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2twlxiqpk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2filndisl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2irofdxwc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kdoknuwz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aasvlrjj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pviilblt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nbwazncd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pienbkic.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nfupexpg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ivguwcyw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fmleuciw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2trtlngla.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dlydstkp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2msloscng.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gfpkyogi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dzobrgwu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yommuekf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vddwzddy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2inzttudn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuptcibl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2arbkvdda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaqjiymr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjodowvn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jsalvqws.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ujvzmsdo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2phbavsit.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkixwdno.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dkmflmwc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2llkgrtpr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hlewbbvg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2votdphfn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckulojlp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mvujvmnm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ovlltcra.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oigyiqnc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kwlglock.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tqnwyvzg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kalheazy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xxkchozi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rboftukj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2obxplygd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vsgpsifm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2edaqgete.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kduigeta.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2srsanpns.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qkdsixgj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2akhyoixc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ykeqfiuf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lpvbpiey.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xzzzeaix.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mjkizgdg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ygqdveth.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hyyopnoh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jqsdxfxw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2umaktcrb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jfcmnkyb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kjflclsc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2abyqcbdy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pqwueiym.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejluomfh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ehojofkg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqluocgy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epuvgytq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nscxriqw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dzoyknmm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ilfbqbra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mmbcqnut.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2clixsnwr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivolcugs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rmvwbsgb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfvdsjq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lqpftbmt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxrpalj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dupcglmx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wqcrtnpp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sysruoyq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ugeqxbzu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mxgyhmjg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rbogastc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jyrsycdd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2msutsrnq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkbaghq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2marsnhog.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hvidwkpq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2odlregsk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2umbobnui.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zsmoxohq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nqhwkwtb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hgzmewgj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2axfglyhi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wkwfiujp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vqndgafm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qcjczrxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2udpsaskw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flovogvr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ogkpbixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wikrrzrt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nzlqjwvh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpbnnft.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2udvcpxzp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nkrdqevl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vzcfyxdt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zfsozwcn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxuhber.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fdaomtmt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qppltrqr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dlhmkyzd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lrotmmgu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2khubwwqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2icsocnte.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jzglarrw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yfbqxtzl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gplfbxaa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2daqucmvg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ioaturxj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kfhtlpov.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lpijwqqu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2frdqccob.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jurcsyrs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zcfxyfha.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qktldyqk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ejltmzcs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xbbelnls.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzdvpors.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bzukcvwr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qwkdmvge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2czozspuf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vorjmtxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vimgdflh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhneaex.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2twzlwpac.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bvrthczf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2unbmicqp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2llflevxn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vidhodyi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgesxxpb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hhfyauww.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slxxtkgk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cnhidvmp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2njyzyqfq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2deqvjund.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2sneyjfxj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgoqvbip.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dykfhwmz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdyewmgv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2avsdlnyn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2slwwcjgg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wszbhjwe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hyqrhnau.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2agunqkdk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mwdxzntg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nrmzmqah.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xgtzxaqo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wvdixpmq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hsrgouvv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sryunvxj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iwkwzolq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jpzimrnb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zkwbgutm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2utslrdfm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fuijxiso.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kwqfstss.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xxqrmbuq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wdmknvuz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zeysujan.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cdbswice.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cskhlkjo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jdogukyo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cqyiwajw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpbedstw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2cljwczan.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tswesljn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dvfomvqn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vujnjdwl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbsfrohi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ladnnnab.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gfydmtbn.html


<!-- 参考信息 -->