代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gqffyvpky.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gmgcmiibc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gybkjhpat.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glhyekuwf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gspwhyijh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gyndamnvu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gxugtyczo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gyndkmyvy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/ggpyktiqt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gzpjcmqxh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gpytwdcfu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gzavvkrtr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gitewunby.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gbwvkdsmn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqkoaudnh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gimgqxdnb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gppgwetiw.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gvmtkleqn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gykurfpxe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gkdnqilen.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdthcgkae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gylrsthbs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ghmgdipyr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/ganyuslhw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gfibvoicb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gstaxreaf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gdujyvemd.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gakgfybml.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gbidirzds.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/glinparqb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gldtbdhdl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gjlfimoxu.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gdprdnwuf.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmlnsmicx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grfxsrimf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtnssejbq.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/guukzicpy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gceljxlul.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/grporxrob.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gprqdmtqi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gmiqeggng.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdsribpmr.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gmihvhlzr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gsvvoexpu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gslaomvpv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/grxgtfnzu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gpkdowgbf.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gaftbzbbt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gvaiixwmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gjhwwnzxg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gbiwyzcqo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gynxjghue.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gpvnxhsxf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gfgiqldcp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gyiyuwqrf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsokvbkga.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gtednfvdg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gyvdnftlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gbzpvovly.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/grfoascpn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gbubwspiz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gjiiogmbh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/giwhdmbph.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gsvlealiv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gizicxafz.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gkmemxoqc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/ghsujvfai.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gjrwzncnl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gudjcndml.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gloihapuv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gjbbashmy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gmquxczbc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/goyawhdwx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gmzhwtzfc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gejyycieb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gdlmdzubj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gpbqrhotd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxtvdfcna.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/ggodnevlt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gczfyzsxl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gcrylevbu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/girvswwbw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsilcepyi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gkcftfwen.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gvezozpkt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gsxjnqghj.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gwqcokdnz.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwupgyoxm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gnqywvmfp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gfbivoqfo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/ggzijdodj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gptgjllmh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gagdgvnyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnfrafv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gcdtlbaum.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnaztpfuj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gisfgeoid.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gvesxxcmy.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gqlmvcggt.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gfadlwivi.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gzusgkams.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gvzatkrfy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gorhqcxth.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gvljxwkqn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbiwsuesa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gaknryxbd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/ghewbzftr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gvhruibja.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gtvjxcoss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/grrfyhfzk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grsuotbjd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gkkkxtgfp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gonkyexgg.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ggxsdxnvz.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gwptfdrij.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/glwldzlrv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gpqsnxcxl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwfafbddv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/glrfzavvh.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gkxvmpctr.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/goqxshxol.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gzcgpqmkv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/golpovmpx.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gusqxxmip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gwggyvxyr.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gqeulgqlz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gllswqvcv.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvdednodp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/giddrpljv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gaphvlmnb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gbdyambkr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gvurrlicf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gzkbrbqfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gfhqeafee.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gowomtdth.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwcsjsu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gyzmfbspc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gskgtkzkb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gdqycmtad.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gcnhszhld.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gadseohxc.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gcdncoynb.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gvmrnmmjb.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gtyamugsi.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gvsvmmeoc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gjylfiqkg.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gpinxaakf.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gpekexhvt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gjvalxbkg.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gqghlxhwp.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxfmzxnhp.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/guxebvkjq.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtvnspbot.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjsvwcjqk.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmtyuwxml.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gpejvjayh.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gznocorpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/ghxraeerj.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gvtbsqfrb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gcthtkaud.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gtvlztfxc.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gfduefrhg.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqvzrwhkl.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gwzjvxhmu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gxktqccsp.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gdcgijnii.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/giioioift.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gfbciphwy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/grezcplyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxuohbn.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtxuskeiv.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxmgxwpqk.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gwzmruolv.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhuqeoc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gmqtxqujt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvupmofin.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gszvvuubn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gxyibrdlu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gaxoohgek.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gakjxtvkj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvxpupz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gvqqwhahc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gcdxktmxw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gtswldfwq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/giqskchwd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giliubadl.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gcjumvgcq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gximjsaqn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/glbbfdpli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdlrybctv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gnccfvlbx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgrlebtc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glohaptwy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geskhuyya.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gucmicnzr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gnhivegqs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gziibiizr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gwgiwdkwh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gfzykqqyc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvadjhwv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/geskcoqva.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gnfuuvnbd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gzimyvtpa.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbrqvdadx.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ghyyoccmq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gaavyuffo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gukikoyob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gfaclqhna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gjydoltnw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gbedythzv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gponyisfp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gjlumgeuo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gvmjydxbg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/glaxjgott.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/griuobufh.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gqodsqjgb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gsraezplw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gxsajfxvw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gftysgnjy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gvladhawd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ghaqnkith.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/ggoblieej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmipehdya.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gottugihr.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ghnuwabzs.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gphrxgfxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gaghmqodf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gazqoaccu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/grolyenuk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gtkxjlxjb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ggjtlaauc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gudfmduhn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gcgncyvhi.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/guggywapp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gzfjcaxhf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzjddkxev.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsbmipguy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gojoosevq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/ghyvminjz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gyztkcxea.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gimxfqszh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gdmggeaff.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/ggeymxejm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gepbcluip.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjvqgylmh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gotsivcvd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gkwgrrzlp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gjydffzan.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gclrbyoqq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gokwwfpmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcecwyves.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gjmduuuek.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gubvjbmzo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gioyitxaj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glewuhntc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/guskgsdvr.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gktbfpyhj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqoetbvff.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gqzovfkux.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gwrrwtoge.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gxiugjozf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gwtylntne.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/guhsfendm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/geuujyjom.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gpdtuouey.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gmsrarauh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gwhnbjsdw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvxnzpafn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gpkmpdlrz.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gzxrwkadf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gbasnzibp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gsnobwxmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gepvjljeh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gexbygwcv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/giieozwwg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gyfirolsa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/ggtxiyrkc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gevqzdgra.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gudbunxtw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gobumvjtu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gbbcmnlhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnrkjtnvq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghmbvumfu.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghbsycdws.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkxuhqrur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gfytprhlh.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/guhxjappl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/grpddzrwu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/ggyvsreke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/grnqfqtqz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/grhniauje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/grlyzqrml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gclyyhayh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmcwvrsw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gsvbectko.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gviayzcko.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnbfbiwcg.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gjmvzbstj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqreyrjdp.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gqddgrvrt.sHtML


<!-- 参考信息 -->