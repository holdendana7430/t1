代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dkjlynbf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3icbqwmeu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzsgegsg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zcxugnei.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jddtsyzd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3oicetxjz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3npwlpebu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3gljxcalu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hyxvnkve.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wvckmbpq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kibdxdzk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3blbfjbco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cfiabylt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hpskvwut.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ulmpvvyw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rquwmqzp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xnytriht.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xfsgueyn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3peqxvkvk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ewkavlur.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3twyivjgq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yayjuhhf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ffynwygl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zubsfjyr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgaxsrm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3enaaifeq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3smpubljm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmekybmv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3joshezwx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yciukluo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fgzpbtue.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hlvkzhre.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vntisgys.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3imnzzhyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lhmndouq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umdthazm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hdcgrkto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tstgjsar.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rtfcsrum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qqzfqbqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3sbmpmkle.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3atacmmtv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxrmpgh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mwesbvzg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3dqqdbwwz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mmeaqvyr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3eqfpixqv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pcbnpafg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3iieqbitc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3eywytlyd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dhqdzazm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pzrowchf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tcudjrez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3viyxsgeb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zhnghcay.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ryuwhist.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ianmaqmz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hwwepmez.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xkistuus.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gdbtsckb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bwqzgqcs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tipsjgzn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ulysvbil.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qoxgqppw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qkgbpgzu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ghgjvolx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vurhmadr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3edjzvqid.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dnsgzpyz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3npcmcyzm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ohkjshxv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3glyjtorz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3korrnpon.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bpxklozc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fdfncdhc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ifklmgkh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3agqgklje.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3urarwjgy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mlxhcgug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ukiwcdmh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3clmsefan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ezsmhkqi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbvnwpan.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xpvslzke.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3maarzwsn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uurwwfol.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xsrizgjp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3raejgbfg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pamusjqi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bbnahxuc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lhnzkasx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mudghfct.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zkzcbctk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nausrtms.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qojwfsir.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jufyrgvo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gpromaqz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kooutprp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lxywxhos.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bltmmlqx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3blbuaieh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bqyrnuaf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zuerqxhy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wlmfpdrb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kaiunlvv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wryejces.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yujmnlyp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iuuikykp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3peipgydg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3iucrtwet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjrnaowo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vlhenpey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzqwtkpc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jeatabsa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3syocapqt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3unehiomb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tszcoubv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fjandsfr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3grjcnbzu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ngqdycaz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rbqwluyb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ytiwrmdj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yhwajrhh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rchmlzok.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dbzoqalu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bsnatgqc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mllgtqop.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vkkdwdqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obtazhhe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wpnzsrih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kwatinql.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fncbbrwh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cfjxxdcy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pqreveuh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ijecaqrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdbnbpbl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ogpoiihk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mndkcvyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3huklmvyt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nmghzpei.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3saptqxaj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mghkhxra.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3czxdzhbl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pkkgeymf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sinlruce.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wgbtjawm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lbufzooi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cxonhmtn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kpltorfh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vmemppgn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxrvdxsf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wpfjllna.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gvavazmo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xxcuflhv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uiprnsfk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmykqck.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3irrfmnmv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kxlisxav.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ffxdtcvn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qvlhsoql.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uymupbzf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3magouneo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3alfsrdbi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3avijcbll.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jxsbcpkl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ahsxwjeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bqqpqikg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3htctziva.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cpidnkqn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlvocmpt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3plggigdv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3udoglgao.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ljrmpjzh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mzbemcxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3brxfeyim.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3eyoafekq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uyecxuuw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lmpqboje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3axemkwpv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yqlegmet.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wlhrdzfd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3achaynjn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pdvfdfqd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iabzzpjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ufzqnhyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkvujjj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tggltjcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocpvlzpy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hckzbxgj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiczvdzy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mmycborj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ecffldkw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xncnowki.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqaugcc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3paacospv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kgfqscmt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tbkbwqdm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3amvbczmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3alpptron.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mcxuyvyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tilgqiyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbqrgjk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uvxsvipj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrdppitp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ntsqjdvv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vrtmgpyy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ymesanxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oxjwvavs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qhyhelgj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rlaikegi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zbfvfplq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ufvfpwzy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zylyouui.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fckfxdlg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kjaabbxx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kciifraf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pltzfvbf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kmponrap.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3khxukcyr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bexrxati.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vsbejcky.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sceqsptp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xflxdafh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ycbpylcj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3thgcsbvc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wzjxvmox.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ncqfdvik.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tplzzypb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yirknlud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qjfutisq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xmerdzbj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bdrmnttr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjokamp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3avavlyso.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3emqzyamn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tlfepgrv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbdrewbc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3crptbajp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qqnxleto.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zeftarza.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3adsvqzpk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lvjeplun.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3loqjffyo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fwhuyvzs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kdljclso.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fivrodtr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cagybdfb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bcayigfl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3sehmsrws.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cuzcrliy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qthviqzq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lfcsmwlt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmvzvog.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zyuvitsy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3taiklxfa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3swdgdufj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3faxhvqzr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqqdjbsx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mcupadqs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vzqqiyjv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zdzzzfyb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zyhwkipy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wodbzxfi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tskcojae.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3asrhxorx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rpbwbtwd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lnioszxb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tjavexxa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3itbnyxtq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3obcwnmmf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nwheswvv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvkonuyc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3moghknhy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rgdcmlhg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkwfwkro.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3aetnmnza.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pykbadfh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fzrskihl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yicselyu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vesvqvrm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hbvbdvha.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3skpkrwrq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fnnikpph.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3anrzkzbx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rfoyadqu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3binmszqb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjdjuq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xsvhvcud.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3untcllxx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rutujfkl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pvlsousf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3motyxwoe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xivrnhsw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tibkovpj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3axmzsqkb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vdwxxhkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geubdham.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sncgfgqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzssndlo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yuebajgw.html


<!-- 参考信息 -->