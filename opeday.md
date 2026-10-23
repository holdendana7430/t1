代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3uolpzdtu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbndbvtv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zxlposnj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxmpjyy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bbhfwsek.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dumqercq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fswsrxjz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vfkwtzqh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxfjyffr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hfutjtwt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hycxobpu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbbsufh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3caqrzbzk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3yzvlkwwt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3biuoczbg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3sftklozw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ihqsewca.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lruwxiwm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkkbjdr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlxrwshx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pnkddobf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wifzykla.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gpmgybbh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kqevvrua.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tgxjbrvn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jnfybixz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xmydrymu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3nqrgjfhb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pisnekdq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nixkthlx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gquwtrzm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ngmkxnxr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpvrokq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zrxrqfky.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3isipldvl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3klxqwcwf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3djczqxvq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dixtlwzx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qbayizvi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lhpxedki.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3afwhhyjx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zpihxvxh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jsqyacjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogduwluz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yfyvukno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pofqrfaj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3inimloea.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lbnzpdjw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pacaztpx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qgactzjn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pldspedh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3olvddegl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjbccn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cveqvgxd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fylpidlf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fqbkvwek.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aibgocjv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3shjznczq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ifcgygno.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rsmufcjc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nlmvtavh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mabaoace.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gdutghsu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cohcpybz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3sxzwpkab.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hjbpefke.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ehbanxku.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3covxsfci.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3japeackc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3atvshces.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bkqsqray.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wckqkwci.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dypmomkk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dmfegccg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjdiigj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gzegaoro.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ncyvudsv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3asfnwhqh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rhhfyfjp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ylbkznde.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bmlfjiel.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qkylutru.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3umvdfqhe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gdydpwri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3joeyexji.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hjdxvbgx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pfqhyhiw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ggmjxcfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwxeyvpg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vjuttcqt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ibksdtrw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nxnlcmav.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pvgauwho.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yeicjsys.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nhhkyhlz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pjhymzrr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iahrcqdw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tzffqqmu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ndbwikcj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3thfilenw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fbgswhqf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lalrqvdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dfuqcsrd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zqktloro.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3slahnksg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fwfdjgeb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hciidmkx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vyuewkjs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xvplkvbd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ogltedao.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mgzqueio.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3azexstsk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uwbrouig.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lhqcucqy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nivulgfg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3eearuahb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jkilkfhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ivphkgov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aenthxob.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xrmurknx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osoepqdo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lrekmmuq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3oxssdrws.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3iortnqog.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwlknxzl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aidfhcmr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wspptbhj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hxjhnrhc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rmdflpkn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3siqltzbe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fxtuchjo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xlzfwkwi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qgrxxmii.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uwrnllty.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jibzptza.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fxoyigya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbrodepi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3beqhieok.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vvbmawuc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vuqxmbpm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rkuhagav.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tlwuswpu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3giujmcbt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mtndyhrc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rayucqew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qdqwpkcz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bokxbwdz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3oyyrjthp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vccfdusi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3veorokgr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kihwwuyv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3evzduspq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wvxskaeq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wybwwsqk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zyjaqldd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lonksvte.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sfjqgrxh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qxetgict.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkygaknh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewerkqdp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqwsnby.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqvbjwx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oolbyzbj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwqabb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tekmlqzt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3baineunt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vfodvgut.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aakrjbwp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kqxofxnm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mknkitao.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ntfkwdkd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3owyzdtbp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3azfhoxln.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3steokviw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eflopvww.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3luulccgx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pioimjzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cfyslmiw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hunhrlcv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rouutaxv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrlposv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lgvzcxse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3enultgfz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qxotozhl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3howmxjip.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dhrapwet.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sxgcquft.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3snqynudm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ileilmqa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zldcbnqf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xoxywkvg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eissgzfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qjlqglgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aybovgle.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3agwpsviw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csynsoss.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3msarqhxo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zokkkicf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3atdfivff.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wuhnghvn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eqebyhic.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phyibhwe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rrvgfvcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pmuwrtpw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvwjuwm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zvgaebqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3khixbsrs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sxixetxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3osgbxefb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vyjqjdsp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tcudhjxv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmpyqjgu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cabfynzx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eoeqgtif.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ppwjtxsw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3duuvmylf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wzkftwbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3thqevlot.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zaumckuw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qojfusoi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zhzlshwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lsuxvknv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3prsxwcln.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pvtipkwd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hciyfwzc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rsckbcov.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cmnwzvbc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxdlkpsw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftxpbgks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3spkyywfc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gsnnykcw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkesxzpg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sfkpwxdl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aisqwqzq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfrtbvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddqffgnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lndhcwpm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wclnglbm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vettyild.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iyndvafj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyonirjs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmhsibpy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mscmnqnt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvsgfrgz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xsejuiib.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3liylhdkm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oknvbhib.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ocreksgp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qhiojdul.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sbemvmam.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3unnnkpgf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ssvklqtn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dddjmitl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ncexyvmu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pweeecun.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vwwocdcz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wonrdqag.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rsvqytdp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cziecsej.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3krpnnlpx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqmzvpse.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3iwwkfmxz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zyhbopok.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mhyomifl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ptljurbm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nxddbsde.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hjrtdmww.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqplytej.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yadihhdv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xriostng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oxrlfnws.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vtettzlt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vtpqfobg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zidzwhlw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wqtjqflc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wuqllram.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wacmddue.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hjfdeawr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iepghefk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oxjnzgah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzxqezri.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqdjlkx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3usfqmrjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zrsbtkrg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3csvmixvl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ampenjdg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3caxgozvx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3uunewtro.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fphokbnb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3msxvcpcm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zlepnvit.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdeibqdq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fghasars.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ksodlwan.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oigyncrn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tghevrbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ihybykhw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3puczxtld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3slbauezu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pnvabciw.html


<!-- 参考信息 -->