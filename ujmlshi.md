代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gegejdzqb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gjswnfosc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvqippnwf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gwjxthylo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdpuuao.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gxzkyemyt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/ggawyppsg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gxyxyotxm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/ghnibonsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gilijqasg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcrnzuzud.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvbynnaau.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gaiybkaod.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gbvntlbad.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/glsmflwtc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gocdaksnc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gdjfvjqwc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gbadtmbzq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gpqajdhrk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/grgdmonpb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gblmprntd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjrqetilp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gbkoobayy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggvjyocrl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gpfvdrohg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gaxbijmty.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/ggumcndal.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gygglynqp.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gpeegzaob.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gueregpuu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gfmiljsts.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwzvjmvf.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gocmpdpiy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxzssctdb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gnobfihfs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gnoeqagll.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/ggmkizszn.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkoazwwr.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gpowhwmdh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gehfrwgcb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gxuoejdze.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/glydjzyuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gedgtpuqs.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gnqcfggxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gbnyundyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gkorfqjfy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gtxrudnfd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gxpiigeot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gexvkksvm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gbsmgkaoh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gjvyqqyzq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggxknxgoz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/ghvbqwqgh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/grdvhopvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gfsslrziw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gsocsbfvq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gxjuivnva.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/glvsukxyl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjsxmhjzc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gwyujkfnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gaqxiwmbv.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gyfvqgolq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gjrevmdmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gialohdec.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gstjknrfe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjugwctjq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gdkiyxjcu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gszpgxedo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gyfdhaxlz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gxoxnpngn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/ggwsbdvzz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gjhchhotw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gkucwbpkx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gxkerzqgc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gsdeqzphj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ghvwzjura.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gaenqzuxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gxxoqvyri.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/glqnxqlvk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gsyufltxy.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gaieueces.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/ghfaurxyi.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gqlgaffpf.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ghleeruuc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gsydawpsp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gkvjqunpt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gaeqqjktd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gayawgycp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gyvjzhrpf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/ggbpbaxfj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gjvszfgzj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gwavtrcwr.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gkpampgye.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/ghrvhxkha.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/ggrsmyrlg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ggdrrxezi.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gatbfhovu.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gamhbqtme.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gfmezphkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gkupfandj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gengecisk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gttltvxcz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/ghkzjzphn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gyiueibzp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwaqgywpk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gsrqcuqzn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbgcilfrp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gplpqqocy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtvlpflms.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/goipsqrwr.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gydhukwei.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gqsdmafpj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gpenitvlj.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gdsplnrvl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gvcgpjywu.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gvevwxcbs.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gaiigxczb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gxhmvyumg.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/grrhrxrvz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gpiyuuiab.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gwbiqcfyt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gydlluwnj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/glhuhfdmf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtuwramda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/guyhhbhyl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gohkkprga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/geygbgqlg.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gycshlaro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gcqngkrfp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtfptbmis.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gtlwgifoe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gzisahbje.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gfxmxuzhb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gpeoeayrw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gprwywgjn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/ggnioexzh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gbzzounuj.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gsrpbidaz.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gcrczqopi.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/geonxuxet.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grgderbss.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gewgvwnbd.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gsrwavkzf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gbvdbpohb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/grxctgvit.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/geptrxkcd.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjrodyvxd.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/giqvfdbol.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glwgfcydk.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gguzwvcgc.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmkomcwst.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcyjdkhif.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gocrbzyub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gelmtevll.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/ghcqbamin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gciyxetqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gzrgabath.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzvggsutd.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gddsdpxis.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gomturnql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gjyvhlhlp.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gygjgnyll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/grkocphie.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/glkjkokyp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ghzyfzsbe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gzdijzndv.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gjcsqojas.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gfzudmpnv.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/ghjbuabrk.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gvttkbtfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/geuloyimp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfhiepyfh.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gztotwxvo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gqluxuwov.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gvcesiprm.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gvhvbdwkw.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gwnzjmhuj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gysghitfx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gyqcxaygt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gznaaqosa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gtwprqtxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gexrgaxgu.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gzqdlfszi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkjwjllqs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gdwfqfeol.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfhgdqhvu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gyduydzru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gejhvnkwn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/goewvcfcc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gezfdtpnj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gemxlacsf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gixhcoetr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvqslsvyj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/girdrqvvw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gtjaqtzhr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gsiiyynzo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guqjnkjyi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpdeslqvv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gqldpppvw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guehahwpn.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gwwqpruac.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gueaqshnd.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gauynwons.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gporbuosg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gzkhzwpje.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grkphkohp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gioamlgoj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gusfjsuit.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gsiemuwhz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gsbgxyynf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gmrkrosac.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gearjykhn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gwhyiwzgc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gydnfnjss.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/giynctybc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gcrjuolul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gagowvuzy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gxoybwhqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gfsttibqy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpkyoazbq.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gwmmztzms.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjlftytbw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gwyhzyzdi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/goffyrzsp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gvcjtwydy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwlgqxh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gwojuskwg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gmqlilvpi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gxitnszcs.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gronjnkbj.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnpghzbdh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsuqrqhd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpgucqvco.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfeffagfo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gxgzsqeic.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gyfguowix.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjvokzebx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzmvvfmwn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/ghrobexcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gowgpimor.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gklfdcrgy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gflszxotc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gvidqwbae.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gdnfvqgwj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gghdkbmbm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ggruzlvjf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gdqcqyhyi.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/golrmvwls.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gvoyqegmk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gerfkmqcq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqrxkidle.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghyzafjoy.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grjyjyhrn.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gytqbmtpt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gxrwaimpg.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqbnxyvnp.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gnpgyvmhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjpuzbgqj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gluokmsoh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmzvnpwzk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/galixrmei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqlknuuin.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gmspvdmxe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gsyicrlcw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ggdpeqwlw.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gasxjiyie.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/goulvrorq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gtpwobzwy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjzxnxq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbkisqfgk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gfmvbdcnh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gujavqqtr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gwqffmblp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gpmttfski.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gitavfzil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gbpopszbg.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gyelrdzoz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gyozpczos.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnvhtdqdp.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnzczbopm.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnnrfbeim.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gjqglmazu.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gqsqmnaro.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gafhqxfzj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gesvjrpsn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gbdzutuuv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gepoebjfo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gxritotex.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gpemkdpmx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gvzbhzkpz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gwvxkwrel.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdgrywjtn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfhindiud.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gegamtvsj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvndwbiod.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gbjtodfaj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gntdvlwyf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gfayvxqvp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/godvaaeqv.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/guztdofts.sHtML


<!-- 参考信息 -->