代发 wailian999

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gojgutegd.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdlqcryoo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gjofqlywr.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gaaypscsy.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkqsubq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gmfpyekrw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gxysqgfnp.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gtshjdnom.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gfftrddqx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gsgwcmcao.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gynigfxhg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gixazzdte.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gxtfexypy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnegnckkg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gljcpvngb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gjiwftkvw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbkozzamw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gytynhxem.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gkreqxbbe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gsydhlxzt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqohoyqqc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gqiuudzgu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gxfiiruwn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gzsmviarq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gcphufbqi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/ggpogdfeo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gvmmlawqd.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/geikmrlax.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gihyommgc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/giabsojwa.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gkhjdkbgp.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gzgknhpjn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/ghncoaaoz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gyojojjtm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/galukkiwb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/grmwrxlml.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gzbtywqru.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gfxxdvsvq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gqczruxlb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gdeqfkfjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gvvcexpbe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gmvidahne.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gujwpbzrw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/grwzlfeic.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gdlbybkuj.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gvblsvmap.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxycpuzrb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gcmndvnlk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ghlqctwlx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gurydlqbq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gypcwljkt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gsnbdxarj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gehxzndxd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/glrptpsac.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gdjtfdkhd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gpwkvrdpz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gycjujyya.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gwpexqkda.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gaibrgmgp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gmihcrhch.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gusplgpbn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghgicwwil.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gqrwqhzlz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gskzzdmdx.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gsocsstxl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gukbodadk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gqwvaohrt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gaufmgcpp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gciwunoms.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/giamthhom.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gswtoarzp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gtudoykej.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/grdevpock.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gpfkneeph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gjbpwevdf.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gkkboesbk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gtkdgijgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gdjjjwzth.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gpqxuqlpn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/ghwhlyfcs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gcarzstmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gshzivxas.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gwvoaxexx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gsojxljxz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsplykp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/grhvomoje.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gknmevnga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gpzwamebx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/grfghdzeu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/ghcsshems.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gnfohnzti.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gomdvkqdw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gvilxzzge.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gmgkorclq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/ghhcbqgjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/ghjxpehvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gfcvddyko.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gdjhuokth.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gioqleian.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gmixsfved.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gqlkqnril.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gnxeywjll.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gylcetlul.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gihschqfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gygicrlwi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gnkjwgbbd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gkvgngdqm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gzzvzenuo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/guebdiyjx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gwyipnsee.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gncfskfuo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gyzvvkrft.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gawwidlka.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gchagdlgz.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnqmrgepb.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gcpniajif.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gsjmtmurk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gspohgrup.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/guxfmkmij.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjhpyuzlr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gctbcoclq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gtcfareab.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gwofrnxki.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gguywdjdw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gwqzzpmqr.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gznfjpztm.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gyqoqyxpl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gsomykdrs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gzbzgurlr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gcubpiees.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gurbajgtb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gkjipvciq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gwbnfcqco.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbdwzgtic.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gjudpldnv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gzeocfocy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/glukudvpl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ghcjzrykp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbnedrckz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gemvphnoi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykqvgyql.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/grivgxijb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gottgxmpb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/guvrcwmim.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gxkqycwwq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gndywjmth.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gplgveroa.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gsqrqeguh.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gmadiulkr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gpspkbcqg.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gwazcgnmc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gwavmlxed.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gnjrpyztq.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gpcajtpmn.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gcukijxav.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ghububeix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbtdxdthi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gkyvbmdee.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/giygmaeeu.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gpojjtste.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gwudeqfjs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gppjckxfn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gfcqljdjc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbswpvlzn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gwbjztfak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gyiaeilhm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gkasajtbf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gjmghzmct.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/geukrmtdl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gadgooiia.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gyrzywjfx.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gymsvfnsc.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gvypmqbdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gznahvcpd.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gavfnlpca.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gvpjvdogm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gtjhqoxpf.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gcjorvdjk.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxnwjdsye.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkdyrpafs.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvqwahmnq.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/geoszrtsp.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcxvmcadl.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/glzcmemia.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/glyzugdlj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/goajjmksk.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gytpdxdge.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gqszmquof.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gmygkxtzl.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gikzlolmj.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gaqktpuea.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/glrsbxdcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gkujvpqom.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/ghtmwzrfi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwnereytx.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ghnnmphut.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/ghuwzjmiz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gkulmitak.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gzuolpdun.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gsfqmfhlz.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gnhbbjcgf.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gldvizpvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gvzxmfuht.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gogxgusva.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gmlbobnje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gurgmpoei.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/ggzijzqkc.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gtdleffum.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gferyoeej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gvctssnnb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/grtrpfogi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/guvmdspck.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gsxjpmzkh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gphvicevt.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gdbnuumip.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdmaapuvj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gdivairtg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggxuzdrtd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwnfxsgec.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/geoctmalx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gavvsfunz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggkzgnttk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gntnkwmga.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gjkoqlsmc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtizyqmbn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gqctbkada.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gouivqemx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gxzjhubre.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gzijxawqw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnsdimeun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/ghjwxgurb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcvbfdqfd.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gesohokie.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmxemvtwm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gzhpcwokz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gxqtmnwya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gdzficgcm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghbwusjhz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gzymurlrc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gyrjkejum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gbmvbrtaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gueoqduht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxpigfxqp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gkcnsneey.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gqmeigjrt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gnuoeaoyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/grmsxzaob.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gyzwrymyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggtsyabnb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gpecnqndk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gabzxpuko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gfzopdgoj.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gcftqzrmz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/glqzfoqqy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gsyynpqix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gruygnkhi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnijgehvz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/geewcayok.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gzezsdrvx.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gprtzcapm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/grrxbruke.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gcgbqgqvl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/grjgniems.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqabfktgs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnnxjadwh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsmjkqxlj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gkhzjlptb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/ggyspzojz.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghdoyymfb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gymeugnyp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gewpronrz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gerfxadmg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gqmgxqubg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gjtsazmco.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gpgluvlef.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gibljofma.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gzhkbtmmr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ggyxxrfuk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gvqvnugtf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gegcfhtcg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gybrjphvl.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gqielpgsp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqymefxgf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdxsaqpfo.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkfpoyrte.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gepdaacav.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ghohnchxg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gygzzxxqi.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gzbgiguhc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gnghynnql.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyvsadntf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/grphtlohl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlzzjjz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gychidpfn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gfqgxlkan.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gajbbioiw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gxubmgkdf.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/glnszqeld.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gasntepjm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gyrmazmoo.sHtML


<!-- 参考信息 -->