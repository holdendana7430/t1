代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtrgiefwxk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtrcnnxosu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtmiukjtya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtynmmkjnl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtcthyzvjy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtjwhwftie.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtuhzacnmf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtpmcvggqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtokvdoriy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtaiataezw.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtzkuuwyao.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtrvrsvyqx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtvrixxjgq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtqiltymot.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtjlakiosw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtoeonmtdr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtdqngwfvy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtbdqbayzv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtijttghnd.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtasjwhast.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtshdkqtbg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gtvdonpswj.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtxunforpa.html

TS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtiocjrlej.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtaeedlvdv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.meibo888.top/gtvjzqddla.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtsifyiwjk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtopfctkap.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtsabmbrai.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtatxfglun.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtgxkudgca.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtmrkrrbnr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtxqjzgnkf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtojbxrhyv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtpczuiugh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gthfivwdnw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtsluswdma.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtsatqwmrg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtaxgeglba.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gtiamnzrqj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtjnsoiipr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtfodpvhsl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtdegjoqbx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gtjcfqoler.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zycfv.cn/gteqtoravd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtshreuaxw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gthsjuiztd.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtppxzcajl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtnrfzcenb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtmgehjotf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtylmzxjvt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gtwelvkxqi.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtmgfhbsbn.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtlbcrumfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtuvdoyhrr.html

================================================================================
来源：http://hz.sweek.top/gthoshgakx.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtulkgngtt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkzrebvig.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtqcvnpfqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtawuzbuzu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtflyjbuho.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtjwntqlpc.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtktkmario.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenlongwang.top/gtjqbpauwy.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gthvkwfuhz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtuqelahiq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtvdedrdlg.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtasdlwtqw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtevmwfsdj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gttpmczehu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtcgtwnwcl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtmnzoxfwe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtfbseejkx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtqkemmkkv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtaniyzoje.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtyafwirnv.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtidkirfzo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtwgrnvhjt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtxkrhbkxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtcblsrlir.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtlhzlocga.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gtndyjhrcj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtgdwwgkwl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shzxlz.cn/gtgjkbwrgn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtweodzjtj.html

[L04] 设置超时
来源：http://hz.nwbrower.top/gtikwfuvzd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sysykeji.top/gtrkjwkxjt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtvkoadmxw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtwntnbuzm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtacvwekdv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtcblhtskv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtksnwddhd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtyxwbtawf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gttsfeqhnt.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtshgsxugo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhoulong.xyz/gtjsbhhrfx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhiwuduotai.top/gtuimvfjsm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtaspfbpqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtzcmbhrea.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtwaabknke.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtzeaflzqo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gticjzhmrf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ppjwa.cn/gtmjivunwp.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtctlvchzj.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtalzzvymx.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtdxugdskg.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtabttzpbh.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtgzsahoal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtkebkedjn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtqsqhxkqr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gthxibzbxv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtpdifsifr.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtsulmrhej.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tianlin.xyz/gthasibeeb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuanzhike.top/gtedelkmje.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtgtyewhre.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtnohorgps.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtvmqfrfne.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtiovyrzgr.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtzkujhxkp.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtwwxiiswc.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gtjmtbrfpg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gthwuhxnkv.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtlmwsgcyo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gttvzjqlnp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtxybqlhuy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fzhhl.top/gtktjodcal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtpfsmhhgv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gtkqrbtyyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtnlvvrrpc.html

================================================================================
来源：http://hz.hammf.cn/gtgoorvsnk.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtdgpugmff.html

================================================================================
来源：http://hz.daxiang520.top/gtnrelwuag.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtcizyjqip.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtxmqkwice.html

PHP:  $argv;  $argc;
来源：http://hz.pengpengdd.cyou/gtcubbtrws.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtmeuojlif.html

TS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtbbgrlclk.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gtmivsxglg.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtrleegstf.html

Ruby: ARGV
来源：http://hz.chenjidiqi.icu/gtvopeeocu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtpwtconpa.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtiygjuovv.html

Py:   os.environ.get("HOME")
来源：http://hz.aibaodan.cn/gtbevctbrr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtnzidvhsi.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gteggjizsc.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtcwitsdpf.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtznjvafqs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtwwjwzgqk.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtyhbytemv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sufxvd.cn/gtnhgfpyzt.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtpnvsueit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtuuefhtjg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtilifveuv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtdneuevuc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtgupyjbsh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtxaxskejg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtcnaauolb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtlkujknus.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gtumdommad.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtcbrwuuzs.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtqlghydkb.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtsaoiwbla.html

JS:   process.cwd()
来源：http://hz.hfpthk.cn/gtzjcnpqkd.html

TS:   process.cwd()
来源：http://hz.ybcxt.top/gtlhckbwqh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tanke756.top/gtapgfrefm.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtkcgwabvz.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtuhoavuix.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gtuzpkqjrd.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtcjvxhbcv.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtwlczwxdx.html

PHP:  exit(1);
来源：http://hz.redwolf501.top/gtvkjtqokv.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtuhermiiu.html

TS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtnzzzeppi.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtekuplkab.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gteuzuuevv.html

Ruby: exit 1
来源：http://hz.smart0.xyz/gtydixugjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtqbycozzw.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gteczzvmxw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtvkhzagxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtraotrwzi.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gteqynycvk.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtgtdldqwq.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gtjpaetfer.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtmnisavsu.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtgxxudujl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtrajgqoaq.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtnnfukdsq.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtkhhlolwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtcdnmtyub.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gthdvjivik.html

TS:   require.main === module
来源：http://hz.zycfv.cn/gtmsfgfffp.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtdldaapci.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gteoxwozfi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtaapyclpq.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gthsbqesfx.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtdkddjgrs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtxvctcnmq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtxygqqewo.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtoeforuxy.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtvvluufej.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtyxtaecww.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtngkrhpvz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtaxcoeqpo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fzhhl.top/gtcaksuiis.html

================================================================================
来源：http://hz.snrcjt.cn/gtphjqdggr.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtuhpgbnmz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkipazodg.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gtaomutwiw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtmkvdgxac.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtzqcoocbm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtnsledqwa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtlfxjxlfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtbcreyxet.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuetiantiany.cn/gtezhcbehj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258888.top/gttnygwspw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtvpngjuqz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtmgaacefz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtufvvhqct.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhiwuduotai.top/gtjsatrpvw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtllbafinv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtrjcwlkah.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtyrhxhtce.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtegzqksly.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtsodzvnvs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtbczfwzoi.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtalssnqak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtarczjooc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtkahwcxno.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtyquwgvvf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtbziwketx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtijvhawil.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtouzexmpc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtfpymqzqc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigfzy.top/gtqtwbtros.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtxjxmwuos.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtaswzbbak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gthrmkrrrt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gtcjhctovt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtqnrjihwx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtxlzislcj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.0kj1m.cn/gtdhpgyjtc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtbnhdfzpr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtddgfmskj.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtcmqvavkm.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtgvkvidle.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxinkj.top/gtmpknzwiq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtcfddkbcy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtoqgaivis.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtdgxcbfkm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtwrgojqkb.html

Ruby: a.gcd(b)
来源：http://hz.cucudq.cn/gtcmytvngt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtqpccnqjm.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtdhvjsfpq.html

Py:   s == s[::-1]
来源：http://hz.cqqwz.cn/gtqofuzmzg.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtsolsmcqa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtownyjbbi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtflaeyjft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtbecuvqvs.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gthhtropqs.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtskfdmbkn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gthfgvohin.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gtgzmehjle.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtkmvhipdc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gttxbbiijz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtgtpwlmjp.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhijiandao.cn/gtqwelcgfr.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtyxxrfowj.html

Go:   // 手写 map[int]int
来源：http://hz.feifeiyinyue.top/gtmcuzonbv.html

Ruby: // 手写 Hash
来源：http://hz.yj202588.top/gtnxxmnyqt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtmniqglni.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gttdjlavvi.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gttrjqbuzx.html

PHP:  // 手写递归交换
来源：http://hz.andypj.xyz/gtrkayyily.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtfzeubwic.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtgswwuucj.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtdiarpmoi.html

Go:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtkymjfxma.html

Ruby: arr.permutation.to_a
来源：http://hz.wangshuangyany.cn/gtgjekvrde.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtpxdyofzu.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtkxkmqrkr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtxvuopwku.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.redwolf501.top/gtmkveauyz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxinkj.top/gtjkjhfljl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtlqiadkoo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gaohongyu789.top/gtlwtodciu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtwxzfbwrc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtvlbrovbi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtxtxsbsby.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtpuhbtdun.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hfpthk.cn/gtwktuxsai.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtmujxxqzw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtcydshvtz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtvmpjsdyq.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gtwxettuek.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtzoszvhha.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtsrpbzvsj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtywsptxxq.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtmvpqnhwf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtiabogojw.html


<!-- 参考信息 -->