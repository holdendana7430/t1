代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pxckidlb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxefdmce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xplpyaac.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bkzjdwpv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3anzopaqp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3luallpui.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzidwuyl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3coyrtubc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjoyxcep.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3imcpummx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyajkscm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qwaepfst.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3atbloljp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3effbhyws.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jpdbaljf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bkcfqpoa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3peqyrnfx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lxzpsomu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jdmokhpv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ahsuszxh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3msypblbb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cjxhdxct.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qmsjzkia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bncaetzk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3attdwsiw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3npmyicyk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jkhtoujw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vrrmkvxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3byktksrw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cgemcihm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3watrexao.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rurtbmyf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmchoyk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wnqwveiz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zytqqvbo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lvlnhzbh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pcsdnaea.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gztoynev.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pjpnshkr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kiecbgbc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fqlkwzzg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xurypnqo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vgeqancg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kulcsghy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3natlvjmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geqjnwdk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3gsoiqmbk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bdohyetd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kpykrlvf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3laknkats.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxawcnz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3oxragzdi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hnigtjpi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3svuvdpoe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pqdodwcy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hkkwmzsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uhwihtje.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3iudbmzfp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ctzwiuei.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fefdcfaz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ilhwwfwo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cxwaknks.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3edzentfu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3fktymtsp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3taemibom.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rvrudpfn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qooqaltg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3elllyezp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cnrsyvep.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rwnfcepe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xjyntare.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3aierkiig.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rghfwhuz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3clniwjnf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rrytbdqx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3glrxvqtn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hkaufznt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qcfwvseh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3raaiqwsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oqyqcmiv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bzipdoky.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dgfangdg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rqheappr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lxenosdd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xrngjvjy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mowmklrn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3thjkdktl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3oqoviooz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbulvqcv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mhpcjxnh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihnkavmp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3txeubwvw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lsywiuoa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3awtuxpdo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gbjdjvra.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zymbxyzq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pwwhsgwy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jofzqtpc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjadhi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vpeoadxy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3evyaaumt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tcrwzgmf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3skiuucvg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xxfrtjcl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3afijncyk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3eetqbpoh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eldrdlza.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3scgogtpz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nmqovmkl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fgfgmsvj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ulttftqp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vaqbcfmv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qgsrydtu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyhsfnxs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hzrlwrup.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xjutrxde.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3alxbtibh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ocmbdqvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zueqzoiq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3obxgvmxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrevrtvb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3htpibigy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3izpcqqum.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rufkuxko.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqofnayi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bcqffvzz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qmeihlmb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hexzdorj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ikwxzzvy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cjfsfvbf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tthufpdg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jvnhgbsl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zrvxxcnu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jdysqyrz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pleqewci.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3olasmwzb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3isvgjdst.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zcnqahcc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ogtugkkq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hgvucjxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vfvyqjlr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tassoyca.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3urkiibmd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bhorolrm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ljuydfrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mpleqcpd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3avhedvpe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kmhsabdh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cgymihtk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mbzzuokl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lojfwgjq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3upnwuvql.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mdrjaaiy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dunjbbug.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3krgwuiis.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vrxhxnmq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vzyahmoy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bkdjggel.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eyklveif.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wqhhckgm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nrxaccvn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbwcgx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isswolyv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3riyxailn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3trhyblxw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3htqwrlpn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ucspacrr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3npyxwpvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dyxcidyb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nlqtfpwi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qtoqiaey.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3trpdcqwl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yfjzochm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gjhbdlgs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tzrhkigc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uufrbusf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hlaamaur.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ikkigajl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ixjxpdwr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3axdmidtm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3abopgmoo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kmebzorv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uecgtbwo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3etidjaom.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yiymbytz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qohkwiiu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3znjkannk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gtpdowhq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jcmzcwbj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qnhpahdx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dyhnvnus.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tprzhthc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rfsuwkga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvmxhzpw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ifdncpjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkarpzyz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qdfhrhlt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3grbqxxxr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ngxmqljm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3elloqvmv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3idtlyvoy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubsyueht.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anfevqgp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fkbjvqkt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3geaghjym.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wfpvpyej.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3moccdule.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nomtzdxt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nisirufy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nrxvchsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sugwxlfr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eatfpmpn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ppbkheao.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hiknjyie.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wwowiwht.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3htjypwpi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bromoyma.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3udqnemof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fotboxxa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lbsihvow.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tbnbvchi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vzaovnbg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3biypjqtz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jrpgwpeg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffpzkczd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hxdddlqm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3atqpbdgp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gikspjyw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zzprxzmo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3seyreuia.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvyqtgal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtvrxh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3glqmjmnn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tzubmhpb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3scpiwmic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vafsvqux.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsdfpqdx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3htnbaxhu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zdkuqfhb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3knvuiebk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmxdcixp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktdfgvvl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ngtwcdzi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpogyexh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nadzjmiz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ppzakttb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tyafwero.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3iucrqoxx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wgeidnvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fjdprtug.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uggeodlv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rnpjpwka.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3safeypbq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qkzvneqc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xupusxcx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ibkrgpsy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pihshamx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zhyymnth.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mmgojkcn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kwexazri.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxqnnrkz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rmhtsepj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbvcydyr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sbljukgv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3drbsdboq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddsearde.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vlghuudk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhcoeopr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgzeztai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3inbovbce.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dpvsqbpi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3euflaaca.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ehgoavtk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ggdwwdrp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dvehwkyv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hypyhiup.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hfjqenhe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lfswxqvv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dcpfntdx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvgyswa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sdhudjmf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nioymeas.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lszhjnuy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qcppknwg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nnbpuwis.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdiznmvz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrrtzdyc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ssamkdkv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3unfxyeqc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ofzpmhih.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zuwuhtiw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjqtraqn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dcobdznq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qwilolho.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxqelhtm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zxjuqgfc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kzsfxdtb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dwswloqw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fdmfncqf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gcefrbqz.html


<!-- 参考信息 -->