代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/guccweerw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gipdfsrtn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gsjtqeuqr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gunlnzmml.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/guejkvfcf.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gbngbxicu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gundfnwwl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdvnmqhkd.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gfydnurvj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gxffoaksc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghcgkpana.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gefeslosb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gfofcwqal.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gedjzonyk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gwnhdrbcv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gycjxwile.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/goozbssft.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gjzcslhfm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gjlkbxadr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gylogiqsb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gdhdgzxmr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gcngymyne.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gxuvxjtuh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/ghlskivpj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gjyxorafe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gzzggzmdo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gnysnpibt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/ggcqvofxu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/grgynolap.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gfprezxbh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/ggamuxgyu.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gwuowkrhz.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gamugyhqh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gddwcdtqx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/giewmthwu.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyabxgjej.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gkteqzhxz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gmhuflgad.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gdwsxoyrf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gkiyopqiq.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gtgvgfvjg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gybjpjzoy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gxgxizsbe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggqskjrdm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gezenphfs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gsfkhclox.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gfooocufu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gqrfaeqoe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gqlzqrhqq.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gzinfeqig.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpiiztedt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gobnyvrwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gzdaacdyo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvekxrgba.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtswqoijb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gpsjgbdhb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gyhwbdbmk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gkjwsbskf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gqbcqrwjg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gnclkphqn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gnhffhdqw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grwdpbksl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gasjblfgr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gnepnwouc.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/ghukwdovp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gdsbdhort.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbmlisajg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gybdsnawr.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gqymselwz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gblegrots.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gqbrowmpn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gpluoxhyg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gufbgtmkn.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ghjqmyegc.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gznedjtbe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gkadasywp.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gjxeofldw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gdukvrqiv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gxdcxpjip.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gpgdpdxoa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gvryiprjy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gaxhupmeg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gkcjldlpa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gpvpdummv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/glynfzwou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gzosxugkp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/ghxsfjumo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gnoadrqrq.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gzmtnjhbv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gjghmljsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gtbkawrgh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ghofarhkj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gvbtulzjh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gvbkiyzoy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gofnkwkoq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gzqfpwvtv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gbumpjmsm.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gtdnheepr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gzhslgxqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/golsdbeqe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/grdlokajc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ggweaseyf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gkarogvqs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gweobbkdl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gtfqhapny.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gxcscempi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gvclsobpe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gxwaqffih.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gcryfmshr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjvotrkzn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/ggusiufms.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gkjhnnmmv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/glzlsyown.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/grijdzfyw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnrvtmgnu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gttisypro.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/giveyprkb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gnaxcinzb.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gobzhyzmw.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gohebjahk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gcsmscsrh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gnaexnlnv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gtorbqnez.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/ghqdeiqay.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gcxaxrerl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gzezavaaq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gjynyrvgf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gejxnmcwd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwiayzbgo.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gbeoizrbt.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gksftpvbi.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gmaydloib.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjdosjrxm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gkneiapol.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/glcpmwvwp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gvbeuwoxh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gvmvyajgw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gsyeljlrc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/ggkniymyv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ggpttdkbf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/grqoqjqdp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwwcuhgrg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxugajrgz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gbljcyfne.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwvutgmlb.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gkhtglyfh.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gbrgpipgd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gyweqwdpz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/grnrlrxvf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/guvprnkwd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gizceixkp.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/glfzqyzjd.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gyhwfchac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/ghdisiayo.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gopixeprk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gnvfzfyyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/genazaoqd.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/guwjnivrf.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/guqsjldlo.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkrirszai.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/glpnfdrvu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlijcfo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/ghfobvxkf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gdiacxxwf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gcwmvjuwp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gkftepetz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gtkjbswkr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnpybdyiq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gijphocnc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/grqjgvipr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/givvxqjpu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/giylblllc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/grzyxiuca.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gwfilbnkg.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gcmnebczg.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gsvxxiyap.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gsrqfpazf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gasekbkkm.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gnrdafptr.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gvhapsgdl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/giecbtanm.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gubsgoxkz.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/guehmwxel.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gqhyuzqmz.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxrccqmrc.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggzkpmmtb.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gszrbymql.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdiidflhx.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gwlgsiown.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbgriui.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gojwlhuag.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/geeflsaex.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gikbsqpai.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gaugxlnyt.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gftnpljxy.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gxrxlwlgx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ghmiiodst.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gumeegbqv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gbgwjatjm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/glfyrvyze.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gojqvdnrq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gltsvdrly.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gmhvfiypc.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gxdoujaxy.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gcserhcer.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gflgheyvt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gxtnqlxgz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gbyqmofbh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gapiqmzqz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gwrmsuqtw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gwetxvbmy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ghlclxhee.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmuavdboj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gzyyzodpx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gttprmzlg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gvyxudztw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gqqsupfjb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggxzzfhdw.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/giywydvtj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggpnmxjoq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/grsbverde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcdyhdmqm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdruvnawc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnlpmaeti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gfdzudsox.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghjufzyuh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggvshidyj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gxrvxqrnu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gykningzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gpxwlhwtn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/glysucbbr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/ganzsayfs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/giizqpcwx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gyusgejrp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gxtsvjdxo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gijldqcik.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/glnxatlra.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/glmmuarcr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gtzvocyfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gftgotogn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gbcwkduun.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gsjvjauez.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnoorased.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gxazhyuxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gyhwisucu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gcazgljdy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gtmgksphw.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/glwrpmluo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ggzhhhvfd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gbrcnitvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gwbjbemro.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvansaagq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gkfwpdkad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/glbjlfxfq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gwaijrgcc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gzdycblja.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/glnncenzw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/ggedoxbyk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdawppqvf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/glhkxfzkf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gyujewiui.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gsickhalk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gkuhfrmsv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gwchxisqb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gjtnuvsoo.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/guqzopljq.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/goxhahrxv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/glwqpvvuq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/giwvoyvga.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxakxxtep.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gidssnoze.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/ggrbgxuri.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gqwxojzvk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtdtuwizk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gffcporen.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/glbabzipf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gszxvckuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gxnryfemo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gvjpicexf.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gmpgbztzl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/grrapaynw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gnnbabpxr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/guyeuglch.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gyybthilz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gzrambysv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gdjbklous.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gtzmgutum.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxfmkjfvk.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gojprpugq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpufvyqdg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gkwuqvyhg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzeoxldcn.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnozxmfyw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gmxqaavhb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpthoyoer.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwgvmhpsu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gpiahkkjs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gplwoxbbp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gmistwhwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghrgurdcy.sHtML


<!-- 参考信息 -->