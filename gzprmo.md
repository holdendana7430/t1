代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3loakhvko.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdpcpfnj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qtcfgflh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bdrbebrl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xnzeyckg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zfttjpjb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ualrtzax.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gokvrrso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jegmntlp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3cxqlkhch.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lquhrdiw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3drzgdafe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3voedgpol.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hwgnehcj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvoqgfud.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lwwliqco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sskkxmuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gqhqnwyf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uiahevkx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ejmhvyxg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3whggogyt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vboeqcfz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ongptshh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nyzkwoju.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qzvkbpsi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jmyytzma.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzvqsxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qqxstrny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vzupmnjb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kwtraspw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3swasxhwr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epmdzcpv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xzxwmtzu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3stapcylc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jjsezhkl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3eowgyjna.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rrbcvbnx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqcnxwte.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rxzdawav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uobqyydd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3cugeldjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbkmspjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sutmzlie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ealtcynt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gfukspsk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gajxlrjy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hcbbcjig.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bcprwfso.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmdhfnn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3umeonjgd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rmbnmsll.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xhxgydbs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lehpnryl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ivrmbwov.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zeuiwksk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xzhqaetu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lcfhwjvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3sxluaqlg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3peukcvth.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffcydcxf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bgfvfofp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fizpeurb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pdxpejhb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wqaxomcd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aeemxpsd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vcvgkjug.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vfuhdizs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gdjstexq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dfmnevxw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ospcgxyr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jwpnlxjq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oaqkhcjn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kpnvixwc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lpthddnv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mjiorske.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ilqvymma.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3milidrwt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nfjfcyqb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yyfbtfsx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3imezglwn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mzttykrn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hfudqpfp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fmbnuprj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uplsexrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vtcokfnb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xnxavmmt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3takdzfdr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rognffbp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3blmewftz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wqkiskov.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uxjzrngk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ojxkatoa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3awqqcozs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hgcmpqqe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3akguvjug.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wwklmojr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3quvwasfv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mfvhppcp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3whezwtjx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ecixbxum.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dgrynyay.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3privjafa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eoanqwnp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3oyqyxwoj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pmemdcst.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3snebzjvu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nzhpbjqt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zxtxvkhm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yylwbgmv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jcrgyzlf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wnoiulqa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rwjoutbk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmztlli.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ukyrlmeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxlhaqyt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3buqvaqfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdpbhngm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3laiefcuc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bjjpdmbk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gexgrdiw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fexzccdy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyojuqy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xdpdsnot.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yfejgkgn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ngevvblc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fixrxcnp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kevytver.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3llbzfego.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bmpodrmz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wocxjjmc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yulhfsxk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ahlrhood.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vaeffoyk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tavbawwq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ocesymmm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jztwlrgf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ubdmvlec.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ybqecxyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uaxpbwqx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vdonkhic.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dswrbcyv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3blhvkljf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cmpbikfa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fqvolqot.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uysoccad.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uclgbpmg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xukpcthx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3twfzfdnb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hqptoder.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nenftnbh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3axhnudqc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dqsmpabo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ebwwbnyf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3phvjtrxs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ztwitdms.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3soqbtuvr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htmbphto.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxibfjck.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3btxdjyhp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3usxrfknr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvtrebhl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yybyazaq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3swfkjqnq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3okckgeug.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ksenjzfh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yzazmbjm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cnjgdzon.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3npgkngqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bhxowfkp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3araoyrmf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kzncpixi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ykjnuuvo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mswbbuhm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3suqugitm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fmnnanxn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qkqbczuu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kmatoryg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pxcdlmgb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bpxvaqox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufasoypb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3aghzdsku.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3icofvaaz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uspnqlzh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oifaxwje.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fbqwmoap.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yfgoqdrr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3guddhubi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vwvhidfm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3giekcsav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cljnamit.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnlrwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxtjgtuh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vihmceij.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eejjexva.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3twllxndj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3svthrtaj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ihfncsvh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3flsuryeb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wwgzqjcp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmfddv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yqfokrhk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vvlawifj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rawxthib.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zfrhksgi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qnichbxv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jysmlxdh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bpnftini.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enmelvul.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ewpxlbpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vgaiyrda.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3azygqpaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yqrzbtsq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3spzcmsda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qbjdxppo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zyitiqak.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cqhxeytt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ylfefivk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3eddyybkp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cpxiothf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gbudvkgd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3msycmpwc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptecmzbc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3olwmbffl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fimkftns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yymqxjko.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cvqpjagu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oavpfkkj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbvpnfj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmbvhs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekigbrey.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3woghjmgr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cbhaxiia.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cddsoltv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jxsgnquh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nbiqiahh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3djixpufp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fnkglolm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hoybmjdj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3coaqmeyi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vxqcxvlj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vtrwxwot.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zezmhzhj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3giezpnop.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xflnbxwx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cvysrwwa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fucvlfzu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3okazfzow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wyjmwqij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3flgvnkrg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bappdxmz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fqdxmxtv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qmzocivs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dsiaikvt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nmziqgbp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fvyupdbo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uxkcptco.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yzxnerkj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ykevolbi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldvmaktu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3luycetat.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ieyiasof.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfxgznao.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kecknpgm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kmxitpvw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cyxcztez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzramlbd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpxyvgjp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tazdoqcy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3iirxypke.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3anntmwim.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rmekvjuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tukdyzea.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cpmecsxj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3erewfbhv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3idleblce.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ykxrxgcu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjfwykt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mpndcklj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtugnrfs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lbfzforp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zbhmitru.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zfxbnzrz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ckpziugm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qdaoxzby.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3haxvttcd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xnxcahku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gutouswy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fnaxmkzl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bftjnzfg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gtocigsb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3elxaidtg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qwyrijfx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hjpjljgo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hwaormii.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3szqrsgyt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3luvawibx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hwjtqhva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3aksmykey.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bdetmdhl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtvmuq.html


<!-- 参考信息 -->