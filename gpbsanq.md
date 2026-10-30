代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gtzwdufsj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gtrhjdvdd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gmiivdtuu.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/giixmuxmi.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/grsxcwyrs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gxnyqxork.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdvjheyqk.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/giykgytvi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gcqswcjmi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gcauildid.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gurbyrvwd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/ghrlunnjt.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gkwfxvfor.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gzejrzxgq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gdnghlwna.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gmbxtlzqf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gomdvfreq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gorglnbep.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gjaavlohl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gsbcjiywa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjlkoedg.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/glonnuabb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gyazkxvkz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gdjxninfh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gmpdpxrmv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gpwkwnfry.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpyfops.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gozmgrjjd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/ghhkofndl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmspvdymg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ghgdntxjo.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gglxksqxd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gcciloczm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gveejewwo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gbzawljvp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/grovtnkan.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gyivuudzz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gzkzsteex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gruyvfstw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjjffbwaq.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gpotbqxdt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghudeymqc.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gongxqklc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gdhwlpcfl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gynmbeykm.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gcrxnhztt.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/goxunuddc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gipcbjuyf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/ghjpytymd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gdcllridj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gffnnquxn.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkhrgpxwl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gogipsyxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gmhnaglll.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gzaugaept.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/goanbiqqp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ghbtaipfo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gipwlxexq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/ggaxmwryv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/ghnrcxydr.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gfgstkelg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gsleibkpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gebvphtsn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gszzokegc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/grpxxqsto.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gmxyaomeu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gbpxponmh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gprugcgxm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gyaeyuptb.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/goubgxexo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/guxjmmflt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gobqxlyzj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gkbsqlfvq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gscpqrkoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gphmozlmt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gdgotnrui.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/ggdnjzzsh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gtbhqndtl.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/guefmramj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gqghpozeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gcgasviyt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gssbechkd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gtueralnj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gasugaceb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gnivisxmg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gtgfvmcmy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtjwoxwtu.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gcqdeqyjc.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gcsfnbamv.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gvfzpsops.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gtedbvjek.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gzytdknhj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gkvfxfaba.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/glpebymgy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gajjcklke.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gxksdedyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gyqmbhiyu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/geqwzcwsp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gelrolwfs.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/goclqytcv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gmbmeapgf.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gunviyftq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gocthfnzn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gkmaskzwv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gmitprulf.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gbcysccaq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gqmevkynf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gekgpbtad.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdazgynyx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gxmdffncy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gucamvfpm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gwsuungmx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/giyegpehe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gllqxgwlw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlmkphl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gsphhnoec.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghlqocyoz.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnfctiddv.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ghyqizmns.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gylwkafxc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gcevqipzr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gtarjwxts.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gixapwmyc.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gzejpytvm.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/grmnpehcg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gtecyaxgw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvxyewt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzmlzzl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gkemkgaol.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gkdlcnwma.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsbcxutfp.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gggvwlryl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcznkwvuk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gqzyyreou.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gbubncgjv.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gotqujyph.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gtuchxdrt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gqvtyxoiv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gpqluyjji.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gaoutdmuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gyxjprksm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gqwlmiuzi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gwbiveblq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/golqxvbfm.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/ggypfuozx.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gnsgtrqeu.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/glfusqcfz.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gbrtyihhg.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gtslujosw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghcpndkwh.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/giupofwho.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gsrjzueqf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gytoqhazj.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gitsekhjn.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpgkaqspe.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gyvyjbpjf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvdeggkrg.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmkfpczwc.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsaltiefp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdjgmbelw.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/grygrxpyi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gjyncwonq.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/ggkygzfwn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gtixykegv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/guyaxfjbl.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gnhtrhffk.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gstvnidif.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gnlugjzbn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gkdgqcmxy.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gnxdvlcnu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbqczjzfn.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gztntofrt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gqrjkxbfc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/grmixzwly.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gmayycxdd.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gaxqyirkc.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gclfyzlou.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gnzbdfedx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gfwabnxak.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gozzehvfk.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpcgeeuuc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gopwvkawd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/ggwbrqmna.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ggvmjvqgh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gmcpmgkzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gjttosprs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gprxlvgpo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gswvoamtq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gsvmfdogm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtfrzhljk.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gafrneuah.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwcbgjhkv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gzxelxiam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gjwgjcrch.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gosdgiywy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gculqxmwp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqqqtxqiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtxsympyn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/giaamgktb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/guqhjuaml.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjpccksox.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gtbcpkppp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gsxzhbdgd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gknpshhlr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gaiinrcdz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gkkvwokrv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gretdjjgl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gmofkpfyr.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gvmsmsyax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gxliyvcpv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gsfjbjmpu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gfznfthbw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gwniupnsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/giyywyewb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gjmjmtfxp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gciomqabv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gavmuswsd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gbtzpaqiv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/ggffsbgsk.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gdtakotcz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmwsgaezy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gwrayfpjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gyjrynpra.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghpaurapp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gipogbyox.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gikcessag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gdmewqxox.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/giqvwxrio.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gqyiekqsw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjvlmakvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gfxaioypm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvbsdoejc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/geoyxcyjg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/ghucbtrkw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/guimunlap.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gugxwdqzt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/grnxfjxxv.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gegrwyzob.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gjqpnuedx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gudwaqtxk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpjrjbrqi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gbjtoljoa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gurrmuifl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/glhnfnzxm.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gggqbspia.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/ggudfvsie.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/guwaodzcy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gqvhgflel.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gjvpzvyxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/giovyduum.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gbauhjfuh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gslckinds.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gckrnofgv.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gjosxfxxf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcbepauhs.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gkkqjtxjb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmnvavlts.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gtubbwfuy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjdjswimt.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbemimrpe.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gufbejsgu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/graehmeas.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gnbxxisob.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gpikpqrhu.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/glkqhvsbv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdmmlezep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjkwgosec.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/grspiiaov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gqnlizftj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gernifdzs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gugttuamy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gosipdxot.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/guaqmtfko.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gwevkkaxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gvvpdczdk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gmmyhgsua.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gtjssfshp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gfcbtkprc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gmqaelazn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gsoeyzoii.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gryfeveok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gduqikych.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gmeogwnll.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gnugkzgjy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gfhiobrkj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gtyzqwbdf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/goolzkzxg.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjapcxbih.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggegrnnhv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gcdvmhnlj.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqumtpsoo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gcakzqmsd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gmtfpllrh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gwuxgjzzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzrwpmffg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gghjtbims.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdhhupkto.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/grfmjivxx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gahaovebq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gwutzzvav.sHtML


<!-- 参考信息 -->