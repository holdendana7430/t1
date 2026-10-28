代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtahrwpbtu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtjuimgjuj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtxhgkgzsl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtlbpawzia.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtrxzllegc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtmummgmdk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtioigyyza.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtnorvfqpz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtyyrwunpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtwibdrycl.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtsnoztcej.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtaaucgcqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.snrcjt.cn/gtukchohbq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtnvduksoi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtbhgiobzm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hywenlv.cn/gtovhoejxt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtqnggtdxw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtvrowbrgi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtskijycfb.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtjnbtover.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtisvykvip.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gthvfbbebs.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtdcyidrit.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtbdoziams.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtielwujqw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hywenlv.cn/gtocmrneio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtksynhskx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jyoumei.cn/gtweryvwgv.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtemirbhrw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dashuyun.cn/gtlkizotmm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gtldjpwtyh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtuxnizksv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtjmivtrcg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtkxykqilp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtrgoytxhd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gthycmiyef.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtjsvhmcme.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtlabdytpx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gotoacloud.top/gtdkkrqdye.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daxiang520.top/gtcjsmjiat.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtnvroeepk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtrbthgvcf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtfahvzslo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangtech.top/gtjxpmjerc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gtppvubcxg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtastugnrr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ivvv.top/gtorwoxfdv.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtkqghzstl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gttorrkkwh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtgclphyxw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtlcfjnarq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtqzcdqimc.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtrvwlbwtk.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtpglutpjw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtbiibtipj.html

================================================================================
来源：http://hz.cqqwz.cn/gtjbiibfyl.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtgdlhucqf.html

================================================================================
来源：http://hz.guannengcc.top/gtqndveubj.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtjfahzszq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtrxfwivxc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxinkj.top/gtiyrofgmb.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtovzkawat.html

TS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtknpgojnf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtvdardhao.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gthniojqvd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinyuanbaomall.cn/gtnavlihev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gttyzidegi.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtijlrelvl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtxyesqrnp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yonumen.top/gtwanzdlfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtpkavvhpq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtbwqdqbzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtkajnsetu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtjpcrcqhq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtebmzuovh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtppaefjpf.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gteohgaopz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtfhnbaihf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtxuabsalg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtznjgbdcv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtzhamnvio.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtlspmtzoo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtcewaanyy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtlohumteq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtpjbyjnne.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtllqbrhye.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtgetfgrkk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtecnirxwq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtmoeezhgc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtqhcgfkip.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtopqisuwq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xylfe.cn/gtrhwemkpj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtyypzewmf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtrwsslkgs.html

[L05] 上传文件（multipart）
来源：http://hz.gogol.net.cn/gtiyuvusln.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtoplvnfej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtxrirbewn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtqhpadeyq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gttlkguyus.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtrqqslzjw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinyuanbaomall.cn/gtqiwbeawi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtygfonlgq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtfkmkgtvm.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gtpxxuthxs.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtqidqpwut.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gttdddlwbh.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtasqhwpgy.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtybfmtypr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ehwqpu.com/gtqlmnmxoi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtyuuuqoky.html

Ruby: JSON.parse(resp.body)
来源：http://hz.0kj1m.cn/gttzoobsbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtupcznvyw.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtvkmoreqw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.smart0.xyz/gtphzxhtrp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtpssvekav.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtzezmhtof.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtsepfhuxd.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtizhqhjgx.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtnadipgiw.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtexkbhwfc.html

C#:   (int)resp.StatusCode
来源：http://hz.andypj.xyz/gtdfedabxe.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtkrbvdxuv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtsaccpwwh.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtfclnmbhs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtdfmvlzoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtkyrrmjqb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtolevnzmn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtmnzcpwys.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtpxvalczn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtkzsmczva.html

================================================================================
来源：http://hz.jqgfzy.top/gtwmaupwer.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gtfmwzfmxj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqblsnjei.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtmmehowpt.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtiqmynbfb.html

PHP:  $argv;  $argc;
来源：http://hz.nwbrower.top/gtdybkuuso.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtblzhacxg.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtxrdlhgbs.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gthgkbvibz.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtusfxjvzf.html

Ruby: ARGV
来源：http://hz.sxryk.cn/gtvkiivddr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtjkgwqmpd.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtwkfknkxe.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtjkstxlln.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtabdfyxct.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtcsvaksec.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtmyuwjssb.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtpgxdxvot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtknuqmsoe.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtsenmwbfp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtqjwtopaa.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtyltklfxq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gttjipmodn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hongshengwenyu.top/gtdcuejhzi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gttucnggys.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtxjtebmdu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtjfkpgdjk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gtyyiyuwtn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtmtpclwsn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gthfvwmyol.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtlqbadiub.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtibphqopz.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtfgshgcog.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtjlfncldo.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtphecnxec.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtoifxrxrh.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtzacfvcwn.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtzubpavwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtrtdsppcv.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtwfmtsyyn.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtvlrueoyv.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtblpvfxfq.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtmyjydtrd.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtsjtgaksp.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtyizddyfa.html

Go:   os.Exit(1)
来源：http://hz.feifeiyinyue.top/gtvwrmrejm.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtggrdipxb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtvloywxbl.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtvqtubmom.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cheryme.top/gtjmzwiupv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtynusdzav.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtpikfmryf.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtqxafnndf.html

Java: System.err.println("err")
来源：http://hz.hysaishi.cn/gtwyupytuz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gthnbgaiej.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtrcekidtu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtjsienzqa.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtscbbsgpa.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtfggsjmcf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtbhbwtnvg.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtlocvwjfg.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtgocmfcyy.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gthcbwpwhw.html

Go:   func main()
来源：http://hz.wangdashe.top/gtxcnyvojf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtpddweodh.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtwfcucfxx.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtulnikosi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtsdxvvepf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gteadexpje.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtqxftbgja.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtizgfqoil.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtlcwsrhkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.redwolf501.top/gtrrjhzhje.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtlnryqnoz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gteriszolz.html

================================================================================
来源：http://hz.aibaodan.cn/gtuljdqlqw.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtdbooorhi.html

================================================================================
来源：http://hz.hnqzz.top/gtimjwmbui.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtqeqrwlqu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtehrtdrom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gtyzbtbxqo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtijyyfatj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtauxwzqkz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtanmyojcl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gtpcuvzwks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gtxicvysyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtzglejtir.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtmmbwccag.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtgxqlafkw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgufenzy.top/gtlxsqiucl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtphkicjnk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtwqdcsqvi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gtznyywskc.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtapgkppga.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtxxjrtvtk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cqqwz.cn/gtmkxqwfwv.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtiwefpuef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtdhvsqjid.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cqqwz.cn/gtrrsapkgh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gttbweyrqm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtovmolpth.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gthhiyuxyh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.smart0.xyz/gtpmdejwhr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigfzy.top/gtokuqxlzn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cashguo.top/gtdocddgie.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtflcouosm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtitkznevv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtctblrbbc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtqllxkzsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtaufjqpad.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnqzz.top/gtfacopdfn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cdnleiting.top/gtvbdsvzsm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtfldiztnu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zdqjudy.top/gtjvkdmvjw.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtebwhxikw.html

Py:   math.gcd(a, b)
来源：http://hz.xylfe.cn/gtixxxmhzq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gtnydxgohd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtavfscqso.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtcwmptkib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtckgmvaus.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cqqwz.cn/gtkpuiwfkd.html

Ruby: a.gcd(b)
来源：http://hz.xuanzx.com/gtoshmuuvv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtocyyoypm.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtbtgbevpl.html

Py:   s == s[::-1]
来源：http://hz.wangshuangyany.cn/gtdxtdvvyg.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtpprznpqj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtfwchjntr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtmtcufmki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hammf.cn/gtbmjurrwy.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gtorabppxa.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtxvgetvcw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtozoepjap.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtrslktqoh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtplmvwxcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guannengcc.top/gtmccwxilh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtymbflgoj.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtitjeglmj.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtfoxffawc.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gtocgtggth.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtdcrbnpyq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtffkndsdx.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtksruxeso.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtzfcrgcfd.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtclfufptt.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtpxvkhsft.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gttoxjwtor.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtjhehxmbl.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtugxoefgo.html

Ruby: arr.permutation.to_a
来源：http://hz.jlsjyb.cn/gtqtsdnfhc.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtgnoohcqn.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtijplrpfu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtbzdnztdd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.snrcjt.cn/gtzbedhycy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.snrcjt.cn/gtjvqxyxnu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtuqvjjsis.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtfsvosgcr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gttbdhrmgb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtqtgxwwsp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.c1oappe.top/gthjznffcx.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtswfxaszp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gteisvxuaw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtqahqcfya.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtfruedmuh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtxpcfmfkw.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtatfyhaoc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gteadkznid.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtslhlrqlq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtioybrsyi.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtacsondcl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtglpwxcab.html


<!-- 参考信息 -->