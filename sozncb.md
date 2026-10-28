代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtkbcddqsq.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtfvtqbmhm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangtech.top/gtwadxtjwt.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtpavkixjf.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtldzwgdbf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtsqjexdof.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtuyguvkom.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtklgxjnso.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtrpvluttr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtxcbslifo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtrapioknj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtnqezreas.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtqjizttrg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtsysfuqjl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtnbedgtre.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtyrjasxwp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtugfgdtpv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtmbjcbzor.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtadbffucf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtqaxhqcsy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtbmumyjew.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtlkyhqosr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtqbcalfya.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtkhhjmmyr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtzdfycwsq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtxuyfzslu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtolghmvju.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtvrvdqenq.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtxqfpsvdq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtbejcagaa.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtppsbneon.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtvofprgqz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtnkrheapo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtvnnbzteb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtyvhqfczu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtifqmormi.html

[K06] 解析 URL 查询串
来源：http://hz.cucudq.cn/gtfkpsxdux.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtnphugjfm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtfrnwueeu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtwvzibhui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtxwnnoevb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tianlin.xyz/gtpnsykjbu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gttlgfosmt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtpybdyhdv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gthfqqwobu.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtcnhyuwdb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtputmegmn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtwzugzquc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtgerpbmvm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtvuqllbsy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtbphzdion.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gzhubu.top/gtgtnbkyyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gtmmeujpao.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gtkqxngfuo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtgkprtzur.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtxxszizhi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gthqkvkipk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtrdflfmkg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtjklyuceh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtqystljri.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtxdaxbxox.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtfeqnrnug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aibaodan.cn/gtmcwptfbn.html

================================================================================
来源：http://hz.snrcjt.cn/gtuyvskiwo.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtswaazhiv.html

================================================================================
来源：http://hz.chenzaomai.com/gtxhyltekh.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtmenhzpqt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtdxiecujv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtwaftvaoo.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gttjmmvpjb.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtwipswiel.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtysnsljmf.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtlauezryl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtgtbfdwne.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtsnngumfu.html

[L02] 发送 POST JSON
来源：http://hz.0kj1m.cn/gtxazixrel.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtkobbwwuo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gtoirzcoyz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtkxguxtib.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtrutqyxlw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.snrcjt.cn/gtmabxwpql.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gotoacloud.top/gtwxniscnf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtxwnjpqls.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtuaztjwtp.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtevvgvgqs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtnwevskad.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gtgtzyyukm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtnfvlvtdw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtrwkgplwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtejlmimxb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gteerhmefb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtarnoaobt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtpqgwipcy.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gthucolavd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtufoghjli.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtoynisjfk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtrdxkojev.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtvgzzhxcw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtonaxfhqv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gttgoxegzq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtrjwwcbdt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gtblulxjmd.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gttholpjmq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtfjwxmwut.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtogbvieqy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtjkhxqbyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtzciwbcxr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ehwqpu.com/gtdwydnjqv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtsotsjjhn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxuanxn.top/gtmjtkdxpm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gtxxcrgmlx.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtforunqdv.html

Py:   resp.json()
来源：http://hz.zhengqikj.top/gtgcucnolv.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtxedunlgw.html

JS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtyfiezmtd.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtkqsvysqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtqjcqiedm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtgsdbmlxm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtjplvdhtj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtgbvaypkb.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtvvmfksjw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtsfvlaojp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtcwfgxrhv.html

JS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtsucetods.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtxxgqvlze.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtfsgwytxu.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtgepjpufh.html

Ruby: resp.code.to_i
来源：http://hz.dashuyun.cn/gtsherxwxy.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gthwxodefo.html

[L08] 并发请求多个地址
来源：http://hz.pengpengdd.cyou/gtsewwizxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtzzpkjofl.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtskfzxjyi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtgkiyhker.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtgldkawbq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtsfenxqwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtculrysxi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtugjevmvc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuanzhike.top/gtmrateayc.html

================================================================================
来源：http://hz.cqqwz.cn/gtduezfvdj.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtutolnltg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvktfymyo.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtryrgcttp.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtcdcugfvx.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtgkkdhdsk.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtxojqvbla.html

TS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtlwpcjuam.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtlqumfrgo.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtibqcptae.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtnuyfyalb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtnxvueuri.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtksgrbiub.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtscadywcq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtosvklxhx.html

JS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtrakoqdpa.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtklsancpi.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtkufmxkvp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gttqvsuzzb.html

Ruby: ENV["HOME"]
来源：http://hz.aizwys.cn/gtqvduazuh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtimqsdxtf.html

[M03] 执行外部命令
来源：http://hz.pycfn.com/gtahqatvpr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtyjsiblvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtcdqgoyws.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtvbecysdn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtczwckvvn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gthgasmwqt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gticraahex.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ywan-chungtsiang.top/gtwvambpnv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigfzy.top/gtxdrpywap.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtzhyaxgys.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtmikvemqs.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtcevmyopo.html

JS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtyplryyat.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtkpxjnpdo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtimeovgzr.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtxynjrhhh.html

Ruby: Dir.pwd
来源：http://hz.jyoumei.cn/gtsngjdhum.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtbfnzydln.html

[M05] 设置退出码
来源：http://hz.daria6918.cn/gtxihvvbsv.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtsywioitf.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtmxpocrsn.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtgwhkilsj.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtdnogbydl.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtudkggnti.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtnxnjunvg.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gthbezbobm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gthdcdmjax.html

[M06] 向标准错误输出
来源：http://hz.chenzaomai.com/gtpiffrgek.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtxkgopcai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gtoqixvxza.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtbvaujegp.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtokawwunq.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtvtioetoc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtvecxqylq.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtjmnmurah.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gtgmztejkv.html

[M07] 判断是否为主入口
来源：http://hz.zdqjudy.top/gtelxavojo.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtuurfxcop.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtqdphajbv.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gthquvmuta.html

TS:   require.main === module
来源：http://hz.shuidangran.top/gtudxxftcr.html

Java: public static void main(String[] args)
来源：http://hz.hongshengwenyu.top/gtanyuswwf.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtfawfzifv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gtyqstroob.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtfvtlxndr.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtdbykayug.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtvhuxexkt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtnrscihxp.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtfktlvnfl.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtirkofjvm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gtjseyamih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtegqtwnfz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtdvfljymi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtofwqrdmu.html

================================================================================
来源：http://hz.svipenyu.cn/gtesepajzz.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtggfkuytg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtdoahtdpu.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtygfljxif.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.birdmap.top/gtqjvzytue.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtzzavpjyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtketcgbkj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtouhqjyvr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtkiprmxse.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtjdfxzfox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtgednrrpe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtvfojhjgj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gaohongyu789.top/gtdubwqrio.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtysejosgp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenzaomai.com/gtwvmtevno.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtthxjdbbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtckweytlx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtcdkylqhp.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gttfkxaxro.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtbbxebthr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtzjolfkve.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtlehxrhfa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtnofmnths.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtqpjjxghy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtvpiqbxea.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtbbfjktyf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtmmasutqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dianchejie.cn/gtgcmaluzv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtiqxamdyl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtxbnyanpl.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtlepotbyh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtkmejoaiq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yanxiufei.cn/gtplboiuuw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gthefumjaq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtnvaqhlyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtnmfeipgy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtjxvwkhwj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtiyvqgorg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtdzpuhtdf.html

[N05] 最大公约数
来源：http://hz.chenzaomai.com/gtzlfvpzzf.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtmuflpwml.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cheryme.top/gtfdjrvznk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gttumeoesx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtmbuaawcx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangtech.top/gtbfarqglx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gttqfwunfl.html

Ruby: a.gcd(b)
来源：http://hz.ywan-chungtsiang.top/gtxvqmpnhk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtmpuqywwx.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtwejowubp.html

Py:   s == s[::-1]
来源：http://hz.sweek.top/gticiowgrs.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtmvxxnqij.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtueeypegi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yonumen.top/gtdejmzifz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtqehhfalu.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gtoqpovoxx.html

Ruby: s == s.reverse
来源：http://hz.feifeiyinyue.top/gtaqatqppm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtkyiasumo.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtajvdtsdn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtlfyeuact.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gtdjmhkqlt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtkgibmwje.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtextnrgag.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtfwyydgpf.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtyztwiiwm.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtgdpvveks.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtfmuvferi.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtrpizpqpv.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtpladsnkm.html

PHP:  // 手写递归交换
来源：http://hz.hysaishi.cn/gtcomkyszz.html

JS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtchglvqph.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtexievowb.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gtatpkvocx.html

Go:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtciabowwb.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gtcunzjnix.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtjivwijgy.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtrplkcgnm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtpewxlpwh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtilpkvlry.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtsxxcnuil.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtnwunhkwl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gttsugqpzy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtphjrpfxg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258.top/gtymzrttho.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtthwssqvc.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gttgzctgwv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtrpwkyuty.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtgebubdku.html


<!-- 参考信息 -->