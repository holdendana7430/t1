代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2olhuxwbh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aepnydht.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ioyiawgi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ihgxaqgf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xtsflsxy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hxhrxvte.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezloxltz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qtdfzqei.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yfgetpbg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qypfeikp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bzdytxvh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2srkumlvk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2zuedpydt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wvkfyjdv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dgcucrjm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dgbpaiys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mojexojc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ewskaoni.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xtmoxqit.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kfkjmrrf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrczphsh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cidmdpli.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jzopmpbj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uuhgtucg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ljwoztpq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyvqxge.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ismzstxu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ahpvnmiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2peddykio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fuocponm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fvvaclkb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2amyktlsf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tuzjgtgb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rrgibcyh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sijwpgyz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qifrzzfr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2kmktpotf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfyfutu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qsmnpwfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iegcxxfw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qvhdonlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukfdvngv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2oqdemmau.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2byzkjdrl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qbhmohij.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dndxgzlh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ffabnihm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2eljelsxs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzmvimo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2yawhzdjr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vccggesb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hbzylxep.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2teoucqfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2opnfulmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2apbanxdp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cprxtsdo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yqdotzyo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2yzvuzrao.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ndbxpxcv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cwmadhjn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lsojepwt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sraxwxtg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qdlkksos.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gzlimyky.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wifdrovm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dziebeyj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pjkovbfo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xhflqzkh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fyfhiptv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vnrmzbyg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bpxpgref.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2htpfpfuv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fsqwqmbw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xrclbstd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xwvcuyzt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xzvzqonr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jnjvaphy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2teupgpan.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uqsxhfnp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wjwwqnmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jxwteycf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yllgvycr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ybqbgzjn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cwlliqlg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xgemjlsm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ppdgesgx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vrnsyozy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2flpbaiia.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dddgceyo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jaxkdjrh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vvxvkgfw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xrfxflxe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mtocqjxi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxluxiw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2adqhjfwg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vbnghbtu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ktjdwghh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qidaamau.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vveltcbb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2exfnroac.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vajwmcyj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qtsbhwme.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxxako.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2duwfzmxc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vjglskgd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2chplwcqy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iparopzq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2prxsxliu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lnhucjfq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lhjtsrms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qeljrtev.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2spgdmtrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ucopyvvm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tnlsomls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipkzsrid.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zuevdebk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rizwqzhw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibtgceyi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zmxcucje.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fuwhgndc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pkljxgjw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfcefzw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fzsfiqoj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vkjeckig.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwcwiw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2beetqnwy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfnyswvj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bclaaxrp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sodopdbg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nhtyzfok.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hvwxgvlk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rgdzcnpi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vhxibtez.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tmtfhbko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lqaatrab.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rqugudtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gquljvut.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kjqejams.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2czltrrcv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2autueuha.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nnzhoyxt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ccguiwxl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qxfvtxfu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2srfskouw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hfsarwrf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oaxgjtaf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mmrnbmwf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dwhizjvw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgntgp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pcnfzvcx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sijzmjnd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ctbdwwbh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fhlkiogv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gtezqiri.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drvrarte.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rcjsgzye.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptroiiqj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imepstwv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wpvziiep.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgjhbsg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2njkidrne.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iubrnyjs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ayrznfla.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wcdwpsgq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bdftserf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zotrfbwl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ohfgftxz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nmsjiesc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2uhmekfzn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bcrgyyeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vmnfasmv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hvorpxwq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hxnxedbj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bkfydxub.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2clprtlkq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dzkjadol.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uydbuyup.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tgfejkeq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zaiszpxg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pmcuaoto.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2skboyymm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2htbizvpt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qxzfrxpe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dgwdzrqn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lsyoxtiz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yrcinkpv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zwvkafjg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lqmeozkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2emhrfhko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cccvwohp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mdkbrdzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncepaksm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hdjmvyik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zczkblie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uhvrbira.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wrgstsko.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hprpaqce.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkhpvbb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwlbhhq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ilphaeqe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vovhjoey.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fbixjpae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2unsjrhyo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2eokoisxj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fiohgryi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oswscnvi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2srnzuhrs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrqzfmuh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bgcqvuty.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kzmebcqb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cxcmkkrm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2odarjqvj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2whpidihk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jqjrbjkm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ibdawhfb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ftaasnhg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rfefsmxh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vijwxqtz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uawlauwk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wfndjtjc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yotwyyjg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fvvjcxye.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dnqpcuxq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfjcpusj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgytnts.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rjvszvwp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rafnvyfw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hpbvaugq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xxjdyfcp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eqzalwaa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2apzkvrgu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxjewcb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfriqeet.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zqfmnotg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqzobvhk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdjpaci.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktbimbrs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2esbyjpze.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hijqkcsb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tdhxmojc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mspoxyhe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tpmfygux.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2sismebkc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cahpfeqx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mexpkhvs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2choyjbgt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wxvtoczb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qbwzbhug.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tdazjeun.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nmgdmezt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tluohgpz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2byzinsom.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bnotaygf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qtnzqqmn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ikffncpo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lwysosjv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftnoiapw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2oxobhuik.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qoebbfex.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lgltplke.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbihqoel.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iqhcbpir.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xaosnzjo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oxvczvns.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kxigydge.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ennfufcf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nhosfshj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gdvnklsy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gnyybszw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2omlmelos.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nwwakivv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zhwmduud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ffcpzalh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2awwundwx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cupaozey.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pdfesxzg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kbghfhgj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tdinfudv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ysrqxkks.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jjqszocm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wvpohotd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2palzvgwz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2elmxvtyz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mjaqigki.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tamiivtq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dzzvoaot.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ncamxvqe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kpgkwfcq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2obbcybgr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bqvlajit.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rynfwmvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uhlpnktk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ipipcevo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iuhbvxmq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ezzljjfg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yuvztllg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ojmljzpt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jpsgykgn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qjqlinuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2owhvqbok.html


<!-- 参考信息 -->