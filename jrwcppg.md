代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gsaanfhyz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gdchwaalm.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gmvgcewfy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsabzhqek.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gbssjafin.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/glotqjawe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gbtjiuceu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gssoayihd.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gtqmndrns.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gfictujwl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/ggbhuqmhh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gtdbsoljq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gozefmbpj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gtlbhufun.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gqosipcpd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gyrzuuymf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gyvnbmvvi.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gwslvqquu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gcqntmxan.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gdxfjkuka.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gihaihqle.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghizwwzpy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnppingxz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gxuerenfh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gonkpbolv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gldnrxtca.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gdskiyqzh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gcuxuwlof.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gtxavxxmd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/goezivwsg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gmjgaomps.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gwkfogcit.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gepfgqynw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gxojvyyxb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxehpfu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grukgxuwr.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gdqwysjuz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaqckhwbz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gdmcsjrtl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gwonwidnj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gijdhxoer.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gvkxbvugo.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ggcefrvja.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gibnumzni.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gonlvrbnr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/grdfzugri.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gzvtzraji.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gycpjbcua.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gzukkhjgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gblmvdfpu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gffgdugqe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gvqcztxyb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gzedhpavf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gpqrcysil.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gfyvlaaoe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/guzaqxszj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gpqbdtifj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxjszvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gjmejeruw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gshxifrwl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gtyojyjax.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gulbsifbj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gluztljzt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gudupkwtb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/guixvxyxo.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/grikambfp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gkpjjvqgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gxqkulszz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/goprqrpfx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gaumkodoy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ggdgsmlte.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/grrcknlkm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/ghblaxoks.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gjrwuxsin.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/genojauit.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gbpcqwjxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gqrpiwtlj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gswmnsxyu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/givzmelbk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gqhjfuips.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gkwpdnzgp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gmnjthgaj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gomtrktec.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gwyzmxavd.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gbaneblhi.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/glkevqdic.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gnkmeojcz.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjikhna.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/grjrvqrlc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gedjagapq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gukqyqcih.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/grecndhvg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gmvhzutqq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/garrcajvh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gaexkfmcy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gvdqnjave.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gpvzxfder.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gherjuxfg.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ghbbzsdnt.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gchpqohgx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gdgfhhyjl.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gwcdinrde.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/ggnfwxoyz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gebozsyqv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpnsjkywq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gtwvnvkkw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gjyegytoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gstkfmkij.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/ghsuixmlk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpvfhdwmv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxufkaszj.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gyzrbhydt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxsxcjbgt.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gozjexomq.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gmnqcpzoj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/giepjadky.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gtjpuvvqp.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gijhfpdfn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/grideqdjj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gohexiuyx.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gkrlviqxx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnermjujb.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggoptggew.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/galqaqbfv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/glbbzhbed.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjxcqlrrz.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gmjywxpoe.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gqprgwmiy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gsjruiszw.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/grpropecg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gjkseggpw.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gtbigsuog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gwrfjhzau.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/grpvieygv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/guchtlrgp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/glwdsdmvg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gidwapbog.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gckjnbhck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gkxpndfej.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/geqrxffvb.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/grqhaoibo.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gdbcooasz.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gvmrhgkym.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxwkxhgqg.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gigdtsfyv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gbzycukxz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghvjauecs.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gevfojfoa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbjdylple.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gbvxrxffp.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gguavohfr.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gmvdfxejf.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwbwregav.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grictvqox.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkjjcsfsa.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gyriotdhe.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gmuhilbdk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gajuwaxuf.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gsvjoimtt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/glyewuyts.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gsdznwqim.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gzieutyym.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gpkbbeqdn.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gggpqeiwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gdxpeswty.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gylfyefos.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/giakldbav.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gwrmqrovg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gzhgbkvhp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/guivgajgv.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gjkdcfxin.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/golomlgnv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gogopniql.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxhqlwo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gsvpqqzqy.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gblmcbtcj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gxqtdbykx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gsbavmvke.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gpqavjnbg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gldltgosa.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvqjtftxt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gkypooptd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gqmhklnig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gteviztvm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gibyfhjtt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvdajuuos.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gdsqduxhc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyeffxgtj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gmwkztlbz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gaxuzcuqk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gdrwnrqlo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/grztuctqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbzrovjpx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glyybpwqs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghissbzxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gjecfpxij.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbclecceg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gwvuyjkyj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/goqnhqvvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfwmqlzfz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gahwergla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gripfgqzs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gekacxkmx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gnlyyqfng.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gezjgdkcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gaabmgvxf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gugakewzg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gewqqyltj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gxlkwywtc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gamkbmhte.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gyqacsadm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gfkiahatq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gdtejyrpe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gyskhfpyx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gygrysjwa.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gausddlrz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/guguwnork.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gwviqezmw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzkcwnidn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkktusizh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmqqyhcpe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gnkedijoq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gospywnhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gohptvsqo.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gdvnrwzyz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/grngydfsf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gbfxhhvqq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/glduhbhgk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gjitkddkj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxuiucaaz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gmspqhpsg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gqsehrwdg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gyvyzzlpx.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gfjxohckg.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gatyhauzh.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gcbwuuvft.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ganqwfxko.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjrcmspbn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/ghbkqdjid.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gwolhirpd.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gwiqeoeal.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gdlwumffa.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gqgxtovez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gxbybsiee.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gshqlteca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gmjmuhvso.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gmrcsjdzn.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gxcmenryl.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/ggxlatgkj.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gvwfkfsjp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gbwsdlxpj.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gualknwiu.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsdbbhjqj.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gabvwpuuo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghyzupnpa.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmxhoym.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gktyamplp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gemonlcxi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gzfjauwqh.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjaposeiq.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gwzbjjzzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gsxnvbzch.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcctqkqri.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdfzxyopf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gbuemfhlj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/guimiwmwv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghgqutohk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gftiplxfu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/grilthulb.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gnyfaywef.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gqgyyeagx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gjdvzjgff.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gmfadircd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gzzpcslfw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjlbgbkne.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gdtwnwyzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gtrtbuppj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gomkggkig.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gtvyebquj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gptcubqio.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/ggjlewguc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvqwuliyb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gaahvkows.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gqpxdtgsm.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gkwpcwuzm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gmidaiftn.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghrmybkqt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gkfzncczm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gfoyibvds.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gpcuggyil.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gakzbiytx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/guvoavgsd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmafeejus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gxgrrptbc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/glqljuwpl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gjentckez.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwtkvbmwh.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gxlnyghqq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grkpxhmau.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gznoaqmon.sHtML


<!-- 参考信息 -->