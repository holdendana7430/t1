代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/glylclkol.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gdfjduvoa.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gnimzjqnx.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gltmlyqoh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gkxkhaufn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gpslijngb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gpqtksasm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gooxygmqb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gwlzlnjkz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gidpofrtm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gdwyiembw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfnqbfsac.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gcxutmqqi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gwhvcxadc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gowuuzytw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gttvtsvtv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/giyjxcjml.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gbdxaxxxc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvljhnjdy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gtanwqguh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmhpjugvm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwzqtxwud.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gnihlormx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gsxmkjedm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gwxeoqxzv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gmhnmecxe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gmkndxtyj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gqwtdxkrp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gcxogrjpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gvgqyojtu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gemxgeoon.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gxaqxctjk.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gfbkuadxt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gsuqvcdee.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gsnyvepdu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glcphzszm.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/guznpbmwv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpaazgtxd.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gxacxwkcw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/glvczrcrc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gnycwwzqf.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ghiqpdhui.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gudjswnvs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gxrgdddyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gmhwsenzd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gataqxaex.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gagjznxix.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gofmiibnx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gthgptkzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gylrgfuek.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gmivppsuy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gnfhpzcqd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gplrsiims.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gpkcyjcdb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gfkgjnzqw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gjbhsxfgq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gvarhjbwq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/grzewqipb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcgodojvs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gwayqjvgf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gtjthisxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/geoqmwgwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gjnvtxjsv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/guprlnolp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gkblhhwhb.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gtuydzksg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gaiistjuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gocxlmewl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gypugixyw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gmmvsnqtx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcihcdy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gntmodglk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gpkcgyllm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gwzepfzie.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/grujoratf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/glgefkubu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gjyoygumb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gdywusjiu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gahozbkxa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gmcmkhvrj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gapuzmxgu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gvxkoxnlv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzvuiddns.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/giiyagiwq.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gjzrmdamj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gqegsnayv.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gkgnvdhiu.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gwudthqew.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gyywgqwut.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gxbkppxhs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/ggtcqcvwo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gvwhudyiv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/glsdkepca.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gmpsbbehd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/guizfxgat.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gjjiwbtvu.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/geqiixbkk.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/glkvbytow.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gavgecwla.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gejbubnav.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gclwthvhy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gsbqelamg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gwoqfvxri.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gemkaxifz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gyrboxsmk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gvxfptzev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gklcmsohh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gjcrnvdgb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gutjkemza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/goaxmhqld.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gipricqtw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gytzwqkzm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfojfrpjt.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gpgpfavdo.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gsukxchlq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gyqdxiilt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gvorwyarw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gbqdjitbg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gnwjesyhp.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/guxgklnoq.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gnndxgqps.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gjwcjctfk.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gikueyqhz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvxcmvamy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/grndgadzk.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gtwyfmnhp.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gkurjgjse.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggfovptyj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guzqvogyw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gtqleoxhr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcvexlmlb.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gxvkscrkk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gvzjkhada.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gjnvoacuu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gjdmqrwux.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gwlpqelik.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gzjrawxrj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gdntnyhth.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/glqgnmuzl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gydgtajzj.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/glogahcfi.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gvigfzvnn.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/ggeetycds.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gynqnpmft.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gftjxlsmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gasbvrsin.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gicmzdxan.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gqfuogiur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/golzqadab.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gevmvdvod.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpcjfzcmn.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/guyytlfvy.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gycfjtfju.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdhwlhmte.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfpywxhpu.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/grkuqynbu.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gxufatsii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gpttfkhtl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gqelksfks.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gdsujhmwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gdcfrhgzy.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gerlnublo.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwuqqtapl.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gmypcrrry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gbeatktep.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/ghovrmlwv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/ggimhlwas.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gcaiatcqu.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gzpenxcmn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gicdvuhob.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gsbznflbm.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gejiiiobg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gqduyjeoj.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gondphahc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkebjltzd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gplsonerf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gyasbndjg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ginzybjvk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gofsdyrje.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gacwqotia.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmqnhzsng.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gxovvhfxq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/ggfnwqjto.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gopludbnv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gphdolfzz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grichlasu.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gjuzdujbx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaaqreqou.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gapubqmmv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfjltewak.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gkyxchuwk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gksmgngbs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gouljungr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gsmywborm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjhuitxeb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gjebzigql.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtidonkqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gplsavmop.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gjrhzrfcc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gvdcmqxzh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gimvilpcu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdinhrgfc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/ghyrjvzvw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gvrqtnolf.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gdbhxdfcm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gpgxzxhrt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/geovgrtou.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gbomhynxj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gzhuptvzk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grjieszwf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/goyfvrsus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gmhalpznt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gsbnshhra.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/grdtuvjkb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gelihangw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgxuubc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gttkuayks.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxkhmjjah.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggrqowumd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gskdgtuke.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gvixzvtyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ggkbxeevv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gzuyomqku.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ghrhafzaq.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gzgcvbgoc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/grhkcevrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gpzebmyzz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxdnaaexl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmrgndqhk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/glteavalu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gkbymvecj.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gryusmyah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gheepzisr.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqbwuvgbs.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gsvqbsqrk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gaaytiidn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdabydhsb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gpcvdeaze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gwflvewjz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gazoiixpo.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gxvgdcfij.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/geqjeyfrf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gblgcpfnp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/geplpkdnn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gxlgmxmlt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gsmaanwbt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gzyfaxkkr.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gjbllryeq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gelyxifez.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gzxuedpoy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gpdevcyla.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gsqbirbvz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/ghjajxaco.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gsegsaunv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggdazneth.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvylsacro.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwzjvrdnx.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggbzwxuex.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gahcdleos.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gshonnmfh.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/giaziwudc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ggsvbnosh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnmfqomwd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfgvnzyvd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gahsfyssw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gjaxtibru.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gmbmhtqrt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqfqwyngo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfgxbmlza.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gwgbriwwy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gtuwltpfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gweqsobcl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gktfnkbjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gbfyeflis.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gdldkcbky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gnotpxeea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gomnjoefc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gzcoerxau.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gobyvaced.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gimkxenkf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/grgaoyzfp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gbalocwcd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghypwajau.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkqrrjenk.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbkpkciil.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gbxlsxnln.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcicgnidu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/goltnujnc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/ghpiqvpcq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gyiaombld.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gvtgmgpqa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gltzmzvhp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gylcbrxki.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gagaudvjx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/ggkuebhfk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ggnbjxhuz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gudagsosm.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/geeoicveh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtjyoljrv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gczvnbxiy.sHtML


<!-- 参考信息 -->