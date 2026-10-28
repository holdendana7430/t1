代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtgphlstjv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtdqpgkwox.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtmfmgzkaz.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtqycliiwr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pycfn.com/gtayirrzcd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtasftecno.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtgashvqka.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtbawlbnwu.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtorqyrsyk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jyoumei.cn/gtkboyxpxx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.vqdsnc.cn/gtunbfxcas.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtgmwacadw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtfcdvimgl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtfjzkbeae.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtebrawlsz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guannengcc.top/gtpibsifgz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtlsbbzemd.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtklddkvma.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtignjzqmo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zdqjudy.top/gtvenslxas.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtwyadxnpz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gthpmywqgb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtbzepkszg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtbdlulvbh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuxming.cn/gtdqkejhii.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtnrolytip.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sxryk.cn/gtjdvpodmg.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtuustwjoq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtdpskpsic.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtxrwqjwpu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtipmkjvbj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtugocucib.html

Go:   encoding/gob
来源：http://hz.yj202588.top/gtbouzvgrq.html

Ruby: Marshal.dump(obj)
来源：http://hz.shangyingyoupin.top/gtfdywdqbx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtcadzeziq.html

================================================================================
来源：http://hz.hammf.cn/gtpstslzzf.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtbyvigzcg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtiujqhzzj.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtvzgtzfsp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gttdwbbpgb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtjdnefplq.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtmvpglssu.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtdyzzzzed.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtpapdbtza.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtebsndvnv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xziqi.cn/gtworhagcz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtutozruxs.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtxjjgzxgl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtulsonabf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtenbtgzne.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtwbigazgy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtzrbvnmug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gthgvbvybv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtcoqzjyms.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258.top/gteonmtzfx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtjsmkshzh.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gttkwugqyt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtjvucyflt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gtzbguauys.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtluwjewho.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtkkbgjcoh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtwpczznhp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtumefqpmn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtzgwlbnoz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtoxtekaoc.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtinwwdfcf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtzzyocyxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtujqmzvla.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtgguvhntw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtbjykvlnv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtxkegycra.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtmijhupgn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.svipenyu.cn/gtynzdzuno.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtczfrehop.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtitidduwd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtgviykgik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gtssumiyvp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtqfdxuqrm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtlhiepohi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guowangkeji.top/gtyrnhcvjy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtnwdzcavn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhaomingkeji.xyz/gtizkefuim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtoxtqurvx.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtrwdgweap.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtuzohmshc.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtipbfjrsm.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gtafcyuiug.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtjgdcfqpu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtakrcuaip.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtrvfulwqg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtpkgyainf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gthccmqlbf.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtiaipsqeg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtisgpmmet.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtvdokxeas.html

JS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtwxdaibkd.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtmepxjubm.html

Java: resp.statusCode()
来源：http://hz.nanxinkj.top/gtloufbqwo.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtrxsbjbue.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtnprbjyyl.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gtgoavihqo.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtmzmvsmkf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtfzkuzwsi.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gtzzpvfeaf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtizfnmlac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtgefeeyqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.mhx1999.top/gtmcpcqcck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtrvyfhszt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtoauwsflj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtrcjjtgsi.html

================================================================================
来源：http://hz.52xcode.cn/gtpctujtzy.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtegglmocy.html

================================================================================
来源：http://hz.bjfxy.top/gtwmjrshgn.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtjemcodpb.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtrjmtcfrd.html

PHP:  $argv;  $argc;
来源：http://hz.dashuyun.cn/gtdlzukrme.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gttjhfkleo.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtkdixdbha.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtjvqkonko.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtctowswtl.html

Ruby: ARGV
来源：http://hz.andypj.xyz/gtblsfxoiv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtpluqmspa.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtfzvcrhqp.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtsufqfmgx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtqbdkrvap.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gteteczpal.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtenpvotyy.html

Java: System.getenv("HOME")
来源：http://hz.daria6918.cn/gtkqvohqdd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtjplikgqm.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gtuiakielv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigfzy.top/gtdvwrddor.html

[M03] 执行外部命令
来源：http://hz.ivvv.top/gteiiqtdkc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtndpsyaeu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtoatjdpul.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtaesveeir.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtikkamqnf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtwxscxfat.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtamvqakxd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gthfcurmzw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gthzuihhol.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtzcyyxovo.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gthqrgaunv.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtiizbtrel.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtpjwakxoy.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtodiptzqh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtoionlcmz.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtnxmurvsu.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gtwvwztwih.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtthbzxozx.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtbyfyufpy.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtbnmnxlri.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtvppddmmi.html

JS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtsxtdbfbx.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtvjivqidd.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtnpkgsxqv.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtavavmhvg.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gtvpibpsmu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtgkaofqsc.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gttcvjdrvw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gteyshijmi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtampobqoc.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtmsamfhxk.html

TS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtguwtsddm.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtfdwiudle.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtfsviujjr.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gtbnupqqvz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtxytoimfv.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gthcysnfuh.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gtkewjpjgn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtcnbxxycv.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtzrmtwgrj.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtbcjhxaqr.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gtctlbajom.html

Go:   func main()
来源：http://hz.quarkkingdee.top/gtebyjivai.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtscsklphn.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtdpzjeeqj.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gthyrlxfsb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtxgplfikc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtkhtspiiv.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtttptzmnt.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtwptafacy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtxauwqvhu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gtqfulvolr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gttwlnmxbe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zdqjudy.top/gtdesydmbn.html

================================================================================
来源：http://hz.nwbrower.top/gtyriqdzwz.html

N. 数据结构与算法
来源：http://hz.yj20258.top/gtidqsrkqd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfptxfaou.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtuignmgus.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtpbspvgvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtsyffukfw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtnhxhyrhp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtbphunbcg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtzolngdiz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtikbomhpe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtdninkvnl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtkzshsypw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtmbxuelov.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtefsjfvnh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtlzsjatmq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtavrklzkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtuxentjga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zycfv.cn/gtqaqlajwr.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtsefugznz.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtenscvcjn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtnpoaayop.html

[N03] 快速排序（分治示例）
来源：http://hz.havefunace.top/gtjgpnlgyo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cdnleiting.top/gtqegoslca.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtjuiwcdbu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gttjojvzpf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtijftsjxm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtvkpcwqrp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sufxvd.cn/gtzdioxqcl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxuanxn.top/gtxxwaacez.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtykrnnqgk.html

[N04] 斐波那契数列
来源：http://hz.daxiang520.top/gtjykbmxok.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtvecxonmo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtccuegzsi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtkonbmbud.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtlqajpfpz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtkvxuhejk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtfbyldvkr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtudjpntfl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.52xcode.cn/gtiirnwzlo.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtokmpenno.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtmagxojrb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtogjziamv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtwzwhpbsk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtbwfryzwg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtgcmaonik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gthfgwvbqy.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtjuucyfjk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gtzgjlwpat.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtglzudqut.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtmqljucqr.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtseymaqkc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtoywmimjr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtlwdaxsxw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gteyivrdin.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtqfcdrxfi.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtbnqadfjk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtxvnkvvih.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtkayxxnvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtqlhqlwjq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtsftwpqro.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtgfetcywj.html

TS:   // 手写 Map<string, number>
来源：http://hz.guowangkeji.top/gtcxgfrvje.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtkftgcfng.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtlvqwnvrx.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtekwgemyz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtqxgxgiwk.html

[N08] 生成全排列
来源：http://hz.yuanzhike.top/gtdjbmroqz.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtqinthrox.html

PHP:  // 手写递归交换
来源：http://hz.ywan-chungtsiang.top/gtykmtccxh.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtbxikochj.html

TS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtkmpxwazo.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtjemxtkmb.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gthgxfwngs.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtacxwkbjg.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtysoayaii.html

[N09] 栈与队列
来源：http://hz.cqqwz.cn/gtsmtzkyki.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shuidangran.top/gtxjwnlwrp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenzaomai.com/gtrebjiorc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtocejehrv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gtiwcgekoq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenjidiqi.icu/gtsfgjbwnw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ehwqpu.com/gtuxvapmxm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gtxfmwryvn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.smart0.xyz/gtbazpqpip.html

[N10] 链表节点定义
来源：http://hz.yongpay.top/gtsapghegk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtgtrbtyde.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tianlin.xyz/gtcjijwzih.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtixahlsyz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtmtvldahm.html

Java: class Node { int v; Node next; }
来源：http://hz.xinyue.icu/gtkyypquzd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sufxvd.cn/gtadffbrfc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtdpepmnro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtipznyfvp.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gthuwcvmrf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gtsoyeastd.html

PHP:  // 手写递归函数
来源：http://hz.sufxvd.cn/gtvwqsnlpx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtyrzykuot.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtzvcvdeyx.html

Java: // 手写递归
来源：http://hz.yvedp.cn/gthqtyhlms.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtlxqlnwjg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gtzopfdirl.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtytkbzjvt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtnwjrzgdi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtxwpjyvqu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtjkvhmhtn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtzwxtemzv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtmqskdhlf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtnceltawa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtzzsiwflq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtbgshabxf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtvtyahfgb.html

================================================================================
来源：http://hz.redwolf501.top/gtexhrbvls.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtljcloeoq.html

================================================================================
来源：http://hz.gogol.net.cn/gtqtfjpsns.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtdwrdyxlk.html


<!-- 参考信息 -->