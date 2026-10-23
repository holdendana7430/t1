代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kcocbtml.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cnkrjzzo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qwovujbt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kbegohvi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vuoqvvyk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nlaxcgoh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3htekncnj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3amviulus.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3heriueyg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdbatb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gxvngxur.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3egmukuyz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qvquvjyw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ghdfjlkw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxkzuwrg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjhsqtfd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vcynjjxl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ruevgciv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3okvugcyb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3royasuqw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zsvrgbvy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfvhcaez.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nvoyridn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3dzlnecry.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kkmwljgo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxglzju.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kotmdnbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nwbtfxtd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nkaefcyt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pmubfmmv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3khdiwpbq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fmooqosf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjmryqzk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jvtafwdv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cowkhgzx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3koltxvqg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mesfdolx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wditujzc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xbyvujrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqsppmob.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pntrpiar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3entzirum.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rxuouvem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3agdoueao.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hqkpohro.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vknvzmah.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uprgueop.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3whutldil.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kcecttpu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ngdxdaxb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wuumzcby.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zvgijhxb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mmcwdlxn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wxvtplrk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rrehqqsr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3usbkqvln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lvftsqto.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3duxazjbv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gpcsnrhz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gvjbxwlp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3uzvcynuh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gbdzlxha.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3iewionui.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3krscezcb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qllhajit.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3szexahod.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eevknyzz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nheqnwgy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3comeybmr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nzqluxjw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cthwyedn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ukzppdlx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wkdoushv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvinnxqf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cuchgsfa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jmyrnpzz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bdlegxym.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mzdlpaks.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dwhotgsb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qglitgpo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ycvmzwfd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ygwoydjf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ezgnqpwv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mhrhkylz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bolijdwe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nzpqngso.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyscaawp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vbfiousi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wxsezamc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvwftqan.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hvlujnfg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hcleukvd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hvoaawaa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yprdcurg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yacelczi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mqyisenz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kfumgyii.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ykjjamxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fsulpvle.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dlbcczmo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kljouefp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zuasqakq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uugcyvfg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lbycneuc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xgvdoyia.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nmwzamjx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ymxnhgek.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fjzpijqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eysxhwuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mrusplmc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3howyclfg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3yutqsayc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zpaylend.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tdzudhla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdvzhhdh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kadvziem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmhjndtx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pzjfbibt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3heiuwdvz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3udqiefym.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ijvucxjk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkxarxpg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3swzjdswc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rnuddlrf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lebclubl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pqqwwzty.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqdbznpu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tkyugmiw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3osoulnom.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cbwqozpw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vkmpuwaq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tvlhblpf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3imhrhfjf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wzmbmbhn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ebhestwo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3swtixbbd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3unomhzsf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tqtkvwil.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3agnnodnk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cuzqtvoq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hzvbdndv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3antteohi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pfmlcdrg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ihnxgjhb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ujtbrjlu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dairoyem.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3goqgbczj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dpxcvnud.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fypghcuc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jotbiajk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uxxzdlvt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xnkippqf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mbvwrahz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lfnvozfx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ykhcfkdv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bkocwsbu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxwoqcd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3psvscejg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfplvlyf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcbahafg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ccyxaqss.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xaqzuisg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pwbupmup.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxpmjup.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rnjgiphw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pytwdgik.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tncaqtsg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3alpnubad.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bzlqzbwa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ethtcgfx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3awnzbiok.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kbkffkce.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3shdscgxz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3izveapfn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hyhbsrbt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fhcqrnwn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sruyqgpa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3oxzhmiak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3netcunax.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cedlyzay.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pohzpnss.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3apapxgfz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kkggwkri.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cypyzchy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hosghioo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vvekfnjd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gxinjbnt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3otuvqmqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3asgxqmzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iodelayy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dbhkhxzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqfhvoon.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gnwljiwd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fkudymbc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wayrlopb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rwlupmop.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wcfolokf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3urpmpycz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ongkkmex.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3thzywktt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sylrzizg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3voofvhar.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jzyfpujw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jpwtnwpa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kreixlpe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oljmjhzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3trkfdnko.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzmjrium.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ovfckqtq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dmbxrqik.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mijbwafe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3szyjnhsx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ceowltlc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vosaykhr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wnkpufoh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ghludafv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3njxwttrs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rcorsjkd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mjuifoua.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3azklalnb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjlmwfhk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pzktwozv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bwurbkha.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qmyivclk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuppkrgb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uvmcgncb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cvsefzjp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pvehejzc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nfccjdvk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjiasoq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3enbdzifx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuithvzr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwzmxnj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kphddylv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3miihvftl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mqpudyda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wvpsgacx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dajqemwq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tjfndviv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gssprile.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aigkajvf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ghdajkfb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cugifnmm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bygmljsw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bzdmxngc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nlmdleav.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3atncgrxw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3msiytcce.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3agfhuttt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3okkmbrjd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xtugsesl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3endynyno.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fenkbcsp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hzchoywh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zxrxmqjz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3grdroxde.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjltpyh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wjijvlok.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ykpqmiwd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xnvjxzcf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sooziwcr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3honkkyev.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3byinqsct.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iohenvsb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ezpdktvo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ubdapqdy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3egblmpht.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cnskulra.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fsewgczi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yavupsge.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3szfdrbvg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iulphyrn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ogchcuaj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gvaufwmh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wovqkjkh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfptbufd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3huguektl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zophbsdx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pdftkkes.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qlliqqrn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kdygagmk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ultafhpx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nirefxqx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eegixvrn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3faeudrcp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qfoxxyup.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fpjxbpxl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvqcsrek.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bfntpiol.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jyguyrze.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nhnukyvz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nlxhwwkb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wkbjrfdl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qlyrzlpf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yhubugux.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bmtlslol.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ebfxdlpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3adrakorc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fodocrob.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tcwtpfmn.html


<!-- 参考信息 -->