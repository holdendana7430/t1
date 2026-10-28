代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtybzvnepu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yvedp.cn/gtkswsczng.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtcjwmxtpw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtfyeeqbzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtuddygzem.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtzpqroisw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtzaaljnml.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtrebcoyop.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtboivtkhk.html

[K07] 进制转换
来源：http://hz.xingfuxueyuan.xyz/gtrsqkqryh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtsuvwnlyd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtwslcyyvh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtcoziaumq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtqcpnrtae.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtdugwnjaz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtyxhwugju.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtcooetpws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gtqbihfwnd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtqstzbkza.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtbfztjyoq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtdaqvuhvq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtyqlczyjf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtiyoehrew.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtauzcwjpx.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtkamlctbq.html

Ruby: Marshal.dump(obj)
来源：http://hz.sxryk.cn/gtbbwxrddu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtmjwqryxe.html

================================================================================
来源：http://hz.svipenyu.cn/gtwjmtbimb.html

L. 网络请求
来源：http://hz.yongpay.top/gtseqlcziy.html

================================================================================
来源：http://hz.xziqi.cn/gtbqzgpphq.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtbaiazlzy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtbhxrgjyh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtgvqzlopk.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtrcockznx.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gtsilbcvmt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gthysxublv.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtvkuirqty.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtzcfunrfd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gtsvkrblvk.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtrkgzfzfi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtdzvffmai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtaryzwxpb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtglrtrlyw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtgjccsvgl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dianchejie.cn/gtiwtpsckp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cdnleiting.top/gtzhdecilb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtysppqqkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gtlymhkgyh.html

[L03] 设置自定义请求头
来源：http://hz.zhijiandao.cn/gtwtjdqale.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtohweaqjl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtbqqtxnsi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtyjpsejty.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtjjntsixa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtomsqwygm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtstbdrxso.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtqjpqkeoq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtyzgmjufh.html

[L04] 设置超时
来源：http://hz.shanyushiyangkeji.top/gtsqrpjdgc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtjstrggtt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtwrntfpsw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gthytrhkak.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtgvblvhte.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtnftvtzhk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtjrfrapse.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtgqeygqxc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zdqjudy.top/gtvfkyvnvy.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtqbvtsekg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtbmpgfjzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtvvcegybe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtkxetkpog.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gttnmbixzl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtpikfmhta.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtmwwovozh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtjuoljbox.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gtjpmhqoqd.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtzjcdyiqv.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtjabxeklb.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtoczljwva.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtvnacokws.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtlaeruulk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtrtuwhema.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtxcodiyen.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtzagaxtfn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jlsjyb.cn/gtufljtiwk.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gtefsbjkvp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtdnptmnul.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yongpay.top/gtectdclmo.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtjmzydbvw.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtnttmtleh.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtuqxxozvl.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtkqmcfqoi.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtvhswszdb.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gturcqrrhz.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtjrpyvody.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtstdwtwzi.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtudpcmeqp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtnuzrpcan.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtkqgjabfa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gtugddzyny.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nwbrower.top/gtpkjpxhtu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtpxpoivvb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtlhquzvnf.html

================================================================================
来源：http://hz.snrcjt.cn/gtxwastqwz.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtjwelkrtu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvzywmdaw.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtgcvuskye.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtqciszafb.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gttabvpzla.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtenptpmqs.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtmotsfizj.html

Java: args 数组（main 方法参数）
来源：http://hz.bjfxy.top/gtivrfboni.html

Go:   os.Args[1:]
来源：http://hz.zhengqikj.top/gtrugdcmoq.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtzkkfzoyr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtjeefvmgi.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtsbbnxcel.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtlvijwgrx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtxhvcjghi.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtiyrppssn.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtfwnpxyxg.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtxjyatwcb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtkgkhknlh.html

Ruby: ENV["HOME"]
来源：http://hz.zhongyouzk.top/gtcjygalqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtgkfkcube.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtmojygrxd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gttspoxjbh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtbcmbqbuk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtvjtdakcx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtrugtmdjf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtvethwbvi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnxiangtu.top/gtxnqprxwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtspeyvqjj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtiryrmadc.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gtstoqatlk.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtaxkgmazw.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtkfmhbxif.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gttmjnknme.html

TS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtfckrtcln.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtfagchlwc.html

Go:   os.Getwd()
来源：http://hz.dianchejie.cn/gthvvhaela.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtqqrpypmw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtydoukkgo.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtrmnjyhnr.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtwvigvoni.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtjecylawq.html

JS:   process.exit(1)
来源：http://hz.nwbrower.top/gtyrnwnjes.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gteljejjch.html

Java: System.exit(1)
来源：http://hz.zhiwuduotai.top/gtvpwgdsrr.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtbhofbcvg.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtowjqrjne.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtsybfsbxa.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtdnytzycq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtmnzuxczd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtarcwbwak.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtezppcibm.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtbrqwyakx.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtadnbkxzl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daxiang520.top/gtdcwxblji.html

Ruby: warn "err"
来源：http://hz.yj20258888.top/gtnlzpytyl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtbmcmxiaa.html

[M07] 判断是否为主入口
来源：http://hz.gaohongyu789.top/gtoutyrshp.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtexoisqxj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtudtpehvd.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtvispzazb.html

TS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtuhuwhddx.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtzgtoduzu.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtuewxlvyh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhiwuduotai.top/gtvlnrwehb.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtkvakyxth.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtugicyxsy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ppjwa.cn/gtszgpqprl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtfhjojvgm.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtghojtump.html

TS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gthitwxdiq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtwagqmysu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtpjdnjzhj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtwlziefka.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtqjghgmrk.html

================================================================================
来源：http://hz.dashuyun.cn/gtvwvqntzh.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtiramleim.html

================================================================================
来源：http://hz.jqgufenzy.top/gtubtpbuus.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gtbedsjzsm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtftbfiahk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gthnavdegj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtphtsokci.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gttevjmool.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guannengcc.top/gtmjzngjlo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtxqcwzkwo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shuidangran.top/gtstulahgy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtkennvvda.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xylfe.cn/gtwtqubalu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtawxfkrrq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtyxcxckky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtsialnxlb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtoyzevxfr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ppjwa.cn/gticbkvucn.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtqggacgpj.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtsumdswkr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xinyue.icu/gtgpxwzlvi.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtnocrwptb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtlyagkvig.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gtxmrjznnw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtcfwkeofx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtplwduziy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtrvpyergf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtsmqjmqsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtkzdkgusq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtiotecotx.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtbchauewi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtkululjbc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtepqzyhjy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtwvhrsuud.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtpjjyfiaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangshuangyany.cn/gtiuzjmmtp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gtvkvjgxij.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gthszanzgt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtslykdfru.html

[N05] 最大公约数
来源：http://hz.ydjk.org.cn/gtyvjxlgrh.html

Py:   math.gcd(a, b)
来源：http://hz.daxiang520.top/gtxzkicwpi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtxoyphenp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtgpcggsil.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtyzsdgkbb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gttubmxonu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtpjnehudv.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtcayxgylj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtswkedjzv.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtoldcmchw.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtiljitoiq.html

PHP:  $s === strrev($s);
来源：http://hz.cdnleiting.top/gtampxkoex.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtxrhikmma.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtennckokt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtqdfzplsc.html

Go:   // 双指针从两端比较
来源：http://hz.cdnleiting.top/gtevrnjrkq.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtfarsuclv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtnkzewnzk.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtdjxxwzud.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gtzmbvhbjt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gtohezczsx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtioquslub.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtcvnezbbs.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtlvzixdla.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gtpqtuljsj.html

Ruby: // 手写 Hash
来源：http://hz.ehwqpu.com/gtyxgwrnnq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj202588.top/gtuehfoxqx.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtkobofigq.html

Py:   itertools.permutations(arr)
来源：http://hz.yanxiufei.cn/gthnmhxhfu.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtxnzcqwbq.html

JS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtlkqsbiui.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtchrgkknh.html

Java: // 手写回溯递归
来源：http://hz.tanke756.top/gtdfsmbyjy.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gttnlixokz.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtnapferel.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtempuhloh.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtowzdrvuu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cashguo.top/gtobixykmq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yongpay.top/gtvkntytok.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtkslrtgim.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtpsferapi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gthrnscfvl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtzppivgly.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtirywpqck.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtstjczmfa.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtlpbgczan.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtuykpmatl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtwjvsjgln.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtfdfnomdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhixingplan.top/gtpcgpsoux.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtwkrsgimv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gthgjawtrz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtusvptmmt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtwdfpzvnm.html

[N11] 二叉树中序遍历
来源：http://hz.daxiang520.top/gtisbjobwl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtaiaunfqe.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtnqtgxhkx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtjwnwaovm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gttnernacz.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtwnttpfcu.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtjstiyeqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtrrbwwsqu.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtqcgqvbls.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jlsjyb.cn/gtutzioexq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtckxxikau.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yongpay.top/gtpsjlejnq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtxsufhvab.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gttgpfhcsi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtryfidvke.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sxryk.cn/gtmfpchprz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuanzhike.top/gtxnchafxb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtzcguuncs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthwmxmqjl.html

O. 并发与异步
来源：http://hz.feifeiyinyue.top/gtaumpbjvp.html

================================================================================
来源：http://hz.sxryk.cn/gtqlhefmfq.html

[O01] 启动一个线程
来源：http://hz.shuidangran.top/gthijrmego.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guowangkeji.top/gtbzsqiqcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtekfuouef.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtxgnlaxor.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtblqploab.html

Java: new Thread(() -> f()).start()
来源：http://hz.52xcode.cn/gtzudlixsk.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtawtkfema.html

Ruby: Thread.new { f }
来源：http://hz.wangshuangyany.cn/gtemtklmsb.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtaickamwb.html


<!-- 参考信息 -->