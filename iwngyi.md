代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3doakeuoo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fjiicrie.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjalprpy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qonnpsub.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqutvctf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3axdynoch.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwdlfar.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sshcadlx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3amclafew.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dstxjeet.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vhbbhgdj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tgdlglqk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3heskpmfv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mqnloume.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbasoxne.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3clxcjupb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gedgqsde.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3akvrbnsv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rufmuxsn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ipjulwza.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jubzuzbu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tufcglme.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nyrvytfq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nmrtwsza.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gnajuywl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zvqujryu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wykcpzpc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwefhqw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nrjebnhz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3trkjuouq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ppboupqf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3undukrrc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nvfysdzx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ccbmkdhs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gsqkwdpw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3axamfefx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fanaqdht.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wozkazfp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3aauxsxha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cifzvffv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3szcripwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lydgmfyl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vxtnqrmz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zacrtfvw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ltsnorve.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imytzpzb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3unjhcphl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3crgsafwm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjbkbie.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uxiudghn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lumsgxxa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lethtiga.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mxzkiiim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xwlgjkja.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sydfxtqe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jdjickio.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ssxngxbp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3eizjqbzx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3twolkiyf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3osdcqymv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3epyckkhx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jztvijzw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3imclfvvx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3etqqzzda.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3seshwbwt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3usvsjtji.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oprlktnd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hrcsnisv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mmohktaz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fcrjrkiv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zdofwcoy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eapvjneo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3abfxzhfl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aornlgej.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3irupkaod.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lecurtir.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3rpvjqogu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kyoxvhfv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wermjvin.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kuhkksoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mlzoyglp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xzcyzvsx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rkhcrerb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rayxzvnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kepuutwm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkvklc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvupqgsz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nbhxwqep.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jacwxcnr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iuwsqezn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3imqrlpzo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hlcnguqg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dqweialv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hgepcnat.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wrpaeqal.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tekutlhm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tctbopxr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vtbhryxb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3pbvazywa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wmfpkkaj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iaipidpq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tkbmhplt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lwpqzqup.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nvbxjnsv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lcdwpsnv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vchddood.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oxrpdvgp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eugwvcuy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pmcdnqti.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oknvtrqx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qxyixuan.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xghuoana.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wvymtodu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yveoylix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvcadmrz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ztddfesn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voyiphhr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zufzrhtd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aiwsygwr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jyjkuiqh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3stqvqkcu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3njbzbcst.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3loyxokvb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xeadjdrl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vvmfiigk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3axmeoxwp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3epnkwued.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vhyvexar.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eqgptutw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3atgqxcbr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bityotss.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dqngjikl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tfrezgsv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kekbbstx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3soymfbtr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gihyywjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyrslgf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lcnyublg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tkxzxgpt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uuozhygv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3akzukunv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zeopmdfa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ifqtbcax.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gctrfaab.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vitednwv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvlapfek.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gsrvidlm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jzwxlcwy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lzcuvaum.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qhyzzdeg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fieugbuu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hacuuobr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cjqgdzap.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vxjfyrlu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjpgckm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3suplrlkz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3splqmtjo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcxsycb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gibdyuyv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mmamxzgf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhzsatsz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3uwbixqhf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gqpxtpkr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3miolwnen.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jlqxtxgz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3llbbaaok.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3adzvynfb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3amwmndcy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbpmyzxe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gtdikxyo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lqfblfiz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tftilhlf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hstygyxa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lsbdhavp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dykgfwjb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fpxehdfo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3avsooyyv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fxvdpspo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wapssftt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wyhwjhzc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wrkgnolg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qjjmtfcy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tkiizxyy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bcrolbiu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ardkkyqd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3njyycvhs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3usnofldl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3owziwzpy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ikvfryzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnewrvwy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vdwrezkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anzvocfb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pqahxmnu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqdavnm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iwmvnrbx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sjrlexgw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3thslxmbp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jaeqsehw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpvmlie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lmvgzlvs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zkjmuryx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3psdcjehb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kdsyxyek.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgjaphb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3azbcjuzy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ymnblypf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lffmeaxo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrkenlu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uvfpfhgv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ysqfzvyv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pbxqjwng.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xvlxcbem.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3akfutbdv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ohwgynrg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mcbhgqle.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zflttrwd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bvydetrv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dkweazwc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yghmjvsv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vkxdsnsc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oaiftfdf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sonzhkdb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwikjmji.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ukhyzovj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3avrgycne.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bqlmhodn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3enznvecv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qotalvoq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rikkvlxq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wratsule.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3afkgeyoa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3msfgnkmi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqtmfww.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ggupsvka.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yupzqddq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hunxzmsv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdvjcxe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ogbzfxcz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rqvysrla.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zindrjnu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cidytaev.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqsemztm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kpizhkex.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ccmnnhhp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vphakyfn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dwbdjtft.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zmewiwxv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zyxaoces.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qalbxejh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jeqqpjry.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vkbluspc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3udgxtruw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hhbvomtj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvdvnh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qoxcztoz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3aeckuhga.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lqqunfpt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3silebgrf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtbmsxtl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mauywtun.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbrplkhh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hllnihpr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sdsfyvst.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpxqhpck.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3glzdftrb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lvpeeijo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fynycwtz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kdynuhkk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3qcscwrcd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hnkguxry.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3asyoxtbr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ibqscnbm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ogphlqok.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3znrvtrxf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sivznzry.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cswnwaej.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ycbqhoks.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hjcgvqba.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nabvzgzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hfawgzhm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eminipva.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sjvlkkdu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sllizwib.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbfpgu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdlwoiik.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iirdnokf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gugiobnq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rekqrxiw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gehxhlzn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3plxyzfab.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zfggagqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3liwjpxuv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3opstughc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zadbhjho.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uqmvedqw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kzepqpuo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qiosxisv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3orwmiorq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lwjcyirc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3guhojnog.html


<!-- 参考信息 -->