代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtcdmihexr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtneibdrse.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gthfiinfyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gttnlqxiwg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtisbtfhdc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtzlverihn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtgvuplapp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gtjzvfmqlt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtpfcrjqvj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtfmcpseay.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtssuepcop.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jlsjyb.cn/gtwpexweez.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtuptfeoac.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtfqevhuly.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtmtuqabsj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtctqvdpmw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtcrcnqgtw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtqvhhkwdu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cqqwz.cn/gtnhnuuolo.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtrxnvatxa.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtywiirlro.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtvqxdsjqz.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtahfuwpyk.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtxlgczjtj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hysaishi.cn/gtnlynxpaa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtikhjbwfq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtpoqrfvry.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtmzyemklx.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtkrlmtabb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtavbipgaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.andypj.xyz/gtjxjmfpvi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gthjxziwhi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtdpdpmovz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtsnbmekfj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gtrppcejhx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtgqifybjt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtaibwqavw.html

[K07] 进制转换
来源：http://hz.jinyuanbaomall.cn/gtsnrpoljd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtcaejiiwc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtqmjslxbd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtuonffhmv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtvphekbrh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtdyxrhack.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtzxnqwoii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ehwqpu.com/gtwdnsgbhe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gthvpcmxsf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gtqaqcywld.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtvetrhtqj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtuvagjjqb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtmmtepciz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gthkiqslri.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtowjlaopw.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtfuvrvifs.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gtforolqhq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtgqcmydee.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcuevoogs.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gttfnmpzcd.html

================================================================================
来源：http://hz.wangdashe.top/gtpamzepxa.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtipwlulfg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtelgcitsl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cheryme.top/gtxjaprxdu.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtuohuwoge.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtutyviies.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tianlin.xyz/gtwmhveqay.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtetckzfzg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gtrwvduhxg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gtbwqwqvbu.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtmxnubduf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtrzsaisrx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtauvlvxuz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtkgyagzxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtiiexfmvq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtfalggwvl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtojhojomb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtsvlpbxtp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtwrkrkbnq.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtkngwunvr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtjccdklxl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtnxtzapts.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtshbjbafb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtfffngegc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtyzmwhciy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ivvv.top/gtkdhihvjl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtrjwymkov.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtzalfjhtx.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gtsdjswzdh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtnpqdsnwr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cqqwz.cn/gtyaykvzmq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtqimckerv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtvyahqcze.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtpimqwmjm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgfzy.top/gtqqturqal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shangyingyoupin.top/gtoylvwtny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtpesipept.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtnuarapai.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtaksqndsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtmzlcjqjd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gticyzmfaz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtcfcdcijf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtlmjxbbfy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtswdogsay.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guannengcc.top/gtlhpvqssh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtkssutfzg.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gtrgyiyrgt.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gthhqsizzx.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gthubsbyhu.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtttpqcilq.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtfsslohyy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtfninzvjo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtocsfnwbx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtogtpohnq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtxipnaaag.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtrtwmwveu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtzoolppzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gttqteinjm.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtimqootef.html

TS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtdwejpzou.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtfvhzxlba.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtmsmqblzv.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtirykuhvb.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtyawjmmjd.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtprrwtemp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtenpfwzkk.html

PHP:  curl_multi_init() 系列
来源：http://hz.xylfe.cn/gtjhubtasc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtsnpztdox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtrwfqmpxm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtlraiqyfd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gttpkrluos.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtxgdocgtk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.vqdsnc.cn/gtumtmngte.html

================================================================================
来源：http://hz.dashuyun.cn/gtpzqzpegq.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gteatrgtoj.html

================================================================================
来源：http://hz.hysaishi.cn/gtjfnenvug.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtzinvkiby.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gtimjxboyh.html

PHP:  $argv;  $argc;
来源：http://hz.fzhhl.top/gtwgkactxg.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtqygcnrfj.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtwjquwslm.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtvcfwuafx.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtwmotplws.html

Ruby: ARGV
来源：http://hz.xylfe.cn/gtuzlbtkqw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtqxuolchu.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gteqlxljgt.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtdxhgwoyy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtmvglpxja.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtgvzloxys.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtlbqtqwyc.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtpfamsitq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gttpbglteb.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtorpklxjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtsygqsieh.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtdtksbzbx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtvyniaryq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtkesdhzcv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gticfavqks.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtrjpsalfb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtnvqfldxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gtkocwtmaq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gthtnxwjtc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtsschtecm.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtqlazbxgr.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtfvuaxwdt.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtmubwaepp.html

JS:   process.cwd()
来源：http://hz.xziqi.cn/gtwvzfveqj.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtusgzzjae.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtswpyefvm.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtdvsqzfjk.html

Ruby: Dir.pwd
来源：http://hz.hysaishi.cn/gtejamapaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtjidtijye.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gtjrpmelul.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtcbeotflm.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gtdgrbdjfw.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtpowuczgq.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gttaaapzsh.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtkjousmvx.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtsvojjhzr.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gteqqxervk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtctpcvrhi.html

[M06] 向标准错误输出
来源：http://hz.birdmap.top/gtaiphlhxg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtsdejyref.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtxluskwyn.html

JS:   console.error("err")
来源：http://hz.fzhhl.top/gtqvcqxxqn.html

TS:   console.error("err")
来源：http://hz.316326.xyz/gtrgnuyrwh.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtaeihejnr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ivvv.top/gtsoiynufk.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gtbykeaeab.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtylljgcul.html

[M07] 判断是否为主入口
来源：http://hz.zhongyouzk.top/gtyddsyokh.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gtbsvdtyar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dianchejie.cn/gtfrtwuvrr.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gtdxmcdwyk.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtxjuwseqf.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtnajzgkta.html

Go:   func main()
来源：http://hz.sufxvd.cn/gteuuhbwyq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtyblhtdjx.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtdglsuteq.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gttshkjcwc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtryonclzn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gtoylzzkuf.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtigtfytsp.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gthtobvund.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yanxiufei.cn/gtegxwqkch.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtzvdtuxfu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtlpxrmbax.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtmvsyegjn.html

================================================================================
来源：http://hz.cheryme.top/gttromwqmq.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtphilzmck.html

================================================================================
来源：http://hz.xylfe.cn/gttisbxajw.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtqulillpp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yanxiufei.cn/gtckdqcegg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gzhubu.top/gtuxcryuoi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtlpyzznly.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtuyabbchs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtiohysfhn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuxming.cn/gtaldkivjs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cashguo.top/gtzsahdhmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtpmnxbjtt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gtceqqckuq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtgkfuyxkc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtaipmpobr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtqabrjukf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtdjithdog.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtssbftrxo.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtrebdptdd.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtaeqvwltd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtdxkmkoqe.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtmeciulyq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtxugxdwbn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtyqhjfxtg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtkepdvkkp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtimigjfrh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtpyvyppjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gtwvikcecl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtntyqfkip.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtaohaslbp.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtcfkjfrgg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtsliqerys.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtjqccvhyp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtawidhwla.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtyewnqzzm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangdashe.top/gtlgpiospy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtuqmseeby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gthvqsmatc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtmpuwekkm.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtkmbwbppx.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtkxoaixdj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.vqdsnc.cn/gtufixvasf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtstmsdjpw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtpzrxirel.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgufenzy.top/gtepkgqyhm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtfscrtdxy.html

Ruby: a.gcd(b)
来源：http://hz.zhixingplan.top/gtvyggohfv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtautswupl.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtwhcmqzdh.html

Py:   s == s[::-1]
来源：http://hz.quarkkingdee.top/gtgmwkfbkp.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtqupmskhg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtnutntlek.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtnuzsbwpr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtxovegbbu.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtduyschqr.html

Ruby: s == s.reverse
来源：http://hz.vqdsnc.cn/gtlyfkxays.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtouczzfsy.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gtdmpbpkgb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtuehmfysb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtavgvoijo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gttkyzqcnt.html

TS:   // 手写 Map<string, number>
来源：http://hz.kuanghao11.cn/gtbnhdajvz.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtnusmaeek.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gtxapqjdvs.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtbjpbtlen.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnqzz.top/gtvydikoyc.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtrlekqxtd.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gtebraztqz.html

PHP:  // 手写递归交换
来源：http://hz.yvedp.cn/gtvzfolcdr.html

JS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtozeltdsn.html

TS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtqlyagkra.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtkzkxinsf.html

Go:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtukwtqimx.html

Ruby: arr.permutation.to_a
来源：http://hz.xinyue.icu/gtvlanvzrs.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtqgifcntb.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtdemjbgnb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtxthfamfs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtilyjmshk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtptffzkwl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.316326.xyz/gtpxcsxerb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jlsjyb.cn/gtsuguqvrc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gthfposbvg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtjffettmf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtinecelra.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtmrzpucxn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtvjfnxsnp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtsiaekrmh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtdlhayxue.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aizwys.cn/gtsjovxhpz.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gtortkjmws.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenjidiqi.icu/gtkbvkjbkt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtvxxqdyoe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.kuanghao11.cn/gtjuerebla.html

[N11] 二叉树中序遍历
来源：http://hz.ivvv.top/gtysnwvbwe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.snrcjt.cn/gtxaxmkxic.html


<!-- 参考信息 -->