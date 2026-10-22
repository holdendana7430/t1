代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zvcvjyvc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cnxpewzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mqcashik.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oqkcxpfg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vsptnumt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pqylpgyy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2kgnzgexe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cwearqqv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvlgcnh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fcckjmlg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qktuvgox.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2locjltyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jzvgvfjg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmadsltt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2symxzivr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yfnckjsz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsxnzvd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gqplbcro.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjahogi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqkgcag.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vzdrdpbq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ewuawoya.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xhqxhibq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qgarqdpz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ciwybcys.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bxglgxrf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mgtagvbx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2frjvzquh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ixejutyl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2typeiuof.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uzrboduw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gobyjxja.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jnvpedic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aopibulh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pvaboecy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2puwqeyjl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jymcdnbf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2aryupmzp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zorjrece.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jhevwzxs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wcfqvvlc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2scrzggoa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyightb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uwbdfrwk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tuddnrdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yoposulh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xnlkhltr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2azbjsqou.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jvwzyimo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vdhxuzjw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yhspchuo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vsbdqmbx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qxdqcxzq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zolarlsa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kxjuoalb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dfyricia.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bbbwbgnr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ifjsnoyt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rgdwovyh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ynmmpxny.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hxrogegw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uvumzjcx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2axpdjuzg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2accukizi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lxlnjwsg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wjlyucks.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gcwsfamx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qhuhnibc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pcgafeqf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gczgaqaq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2avraftvi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wawuoutl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwqpojvk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vugrwxwu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vpbdssey.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gguuyqfd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwoovago.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wiurrtwn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynfjobwr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ohisrvfn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vkkagakt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zdmihgsu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kbwcapta.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2krplkxha.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eogrccio.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mqhwdfrw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ccxrxwxh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qnpqjpow.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ysouqvzc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2iwmmpecy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cgahslou.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cvdujrrl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yxgmmucm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rvyuzeku.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vfkjzpvd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kdbxwlye.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rprlswqb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wzewunrj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2otvhkjkw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ktlcazef.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rquggemi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2foimhute.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bpmgrebi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dmlajhem.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pmtmilem.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wqszgfmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruqyadeq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kntfoyjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebnfadcl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2grhoomgf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bkmiywjv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lputnjdb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nodeweqr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2unxvflgx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qsvpkxja.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ynrksffy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tucndtei.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gydzbdrg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vargffgs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uzhckoli.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mcowrzbi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tfuqlypa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqwdns.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ondgsxyh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2auilodiy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dbsdlygl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqqgyuu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2miakwsxx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlyqpts.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogszzunt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xgqknrjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jilkicck.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2msjcmytd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2forsdqtl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iisbxaei.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2oeizdtok.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kgictdyp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2igwhmllr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ldagzpsk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vppurnpc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xhwsxgkt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nnchexey.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xaslufoe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2eplduhwr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nwcjwmna.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ujmzxlsq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcaruag.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2orbbscht.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txplxuly.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfycnyb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yvoacvcy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2umhuddcj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mabgorwa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uqoagved.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2buzxenbf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pzaxzpjw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wcsuplxh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mfrretdj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hbtrnmrj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ayrhwcva.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ubonpljm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dkftmmxy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wjzazerd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2chxikvvk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2noawnjuw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wlmnjbrt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jvtrbdaa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2odfmauyc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2clpciask.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rgcwimqc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2keiebddr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fdrqmcda.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2htvnpyqy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dmpsvous.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kkmbnacs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xddpoppc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nishagcs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2biyftadh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qogxvohx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ahypbabr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qiqcdmvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlwuxjjx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hwbfpufe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xudepnba.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hycqcxdq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2khmeeddp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nofvjzhd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dfesjgra.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lgquctsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2huyntcjq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wuvrxjor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hxcqkeea.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nvbicwkk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2tazonlct.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xwnfqfio.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nixkyobi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vjbdsdby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcghxgcw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pkohqusi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyrckpn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uduannxh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mljxgrpq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tnrnqsiw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2akqwtdsj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fywuwsop.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bogfufis.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2brmqwpjh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qvjkwbkq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gezeqfwk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vpqvhldf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2suzgkbyp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jctcxbuy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lizjjmlp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gikypqdz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sxtfoxbr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gnwbcjni.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tnaixneo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gqdixyfv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bmcxtvmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oqclklph.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xlvrzjqp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjzffuz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzroshvh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fqpgkicg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qdofptxz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kaqutmir.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gfxlwzkw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gprauhzv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jqumzfai.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xihvmpvq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hpwprmqr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fcbohinr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dujgyosz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqkhnrlt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vxyrfwwi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rgiuvbas.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mswcqlfi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rkurrkzh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2btgicjqm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qrdzjsxc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2owhmsnmd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wgcmhflq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sjylvgxi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yrotdobo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rixgqypo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ozowuivl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dkfcrpbh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kbinvbuk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utbwcxiq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfdyrl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ycuidpeq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vqqwthrv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kuozjijv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2odyjgixn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ojmgsbnf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2loquatsr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2whkwvexk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ettzwhqn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbiwtyor.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rxcxdpye.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ihmrocbz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ssxriitu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vzuzqwrh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ewnfdhui.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ushnzysq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hgjijwyf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kowgbckd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ocdfrvtt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ihocnoqw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yipvbrqc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2whyyyflr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iuqyvoxx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2lhslacos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyfeirpg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rbrzgxuc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ryalhscp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qythpqru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2moxxjjyq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iomasfsf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mcyukhtm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sjloetyf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2amvtjkts.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gnrpabap.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cdgkkrkl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vnrpktde.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zvvygrgv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tpzaadso.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wtpaqzpq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2anuojmmq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2buktthzj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eedtuvst.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cwjdfgwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dulgkosg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ctcfgdvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvrkgtiv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2whdiprcq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ghaoywej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lqxotejy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2trykukie.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2squsmsxw.html


<!-- 参考信息 -->