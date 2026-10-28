代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtqlvrmzdl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtrhfofsen.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xziqi.cn/gteeiunrvc.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtybdqwjna.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gtylxggnsz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtcvmdnetj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtlifkkmxz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxinkj.top/gthanbhgxj.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtwidbyrpt.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtqkvpawxo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtvojbdqpm.html

================================================================================
来源：http://hz.gzhubu.top/gtxmgqhbxe.html

L. 网络请求
来源：http://hz.wangshuangyany.cn/gtckcsyauw.html

================================================================================
来源：http://hz.meibo888.top/gtbqalmnyt.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtxttzwlyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gteyeqcqsq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtshiapzam.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gthrckdrel.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtujcvbpdr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gtxmxqaxrq.html

Go:   resp, err := http.Get(url)
来源：http://hz.tian-w.cn/gtstyfdaum.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtkwnziudn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtpdyomwzh.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtfltbttuo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtqhxpeagc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtybasukvh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtoluhvsvu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtpcddcpse.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtqubjxmxd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtvipukfap.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtuaejtfuc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gtuwnhjuhb.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtaoainapr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtlogkvtrg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtzdykblof.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtrpceejjj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtprnnfjrj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtekzwtrqk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtmdzagrvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xingfuxueyuan.xyz/gtfqotcyec.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtqwhuoszv.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtuyiidzvh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtbwxhupvg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhongyouzk.top/gtuxrzrjdo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtpetnkgqr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtepiteqsd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtmimfuwag.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtcwmnbuuw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtmquowtkp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtmwaqandc.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtssfbhffd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtkntbfrol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtoegbptvm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtlxlbyfmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gttafiqzqg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangshuangyany.cn/gtinljngwg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtcmapfpue.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtiqtwsxda.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gthxhenvnu.html

[L06] 解析响应为 JSON
来源：http://hz.ywan-chungtsiang.top/gttaragdvb.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gtezwrdlos.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtchvitoku.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtawnrhbmb.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtzoabiiyy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gtaigwopbb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtrssphkos.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigfzy.top/gtuyjnrhlv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtjyaxcwdp.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gteyykifsu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtfqoaxrli.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gtiealdxlz.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtbsnaukcc.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtsoyibitb.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gtcunzmuox.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtoergbnwg.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gthnufcuoe.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtkwqklmco.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtxbvaridg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtuueyoeqv.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtaybacqgz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtyivtuhsg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtgvfadfrv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtcjnirdac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtnapuwtvk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtndallfry.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tianlin.xyz/gtkhqpztkr.html

================================================================================
来源：http://hz.hnqzz.top/gtlzjwdorq.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtpxsbwrqc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcjcnpfyp.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gtchcejexd.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gtbopkpknj.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gthzsdbdkj.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtqypeyncu.html

TS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtrntsoxqn.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtbjfrsnbz.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtzpmqzuod.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtixrwusdc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gthmhkebiu.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtlxwuajvs.html

Py:   os.environ.get("HOME")
来源：http://hz.vqdsnc.cn/gtdipascrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtdkxipdvx.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gtzpnuhojs.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtsyphaydi.html

Java: System.getenv("HOME")
来源：http://hz.ppjwa.cn/gtnqugzblp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtplljattc.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtpjlcweuk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gthosbffiy.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtmxkbopsi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtovqmxomw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtmcvuyayj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtheiovlue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtmmlcvrdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gttqxqzwuw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtetqrucjc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtkqfbnzju.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtxjxdswqy.html

[M04] 获取当前工作目录
来源：http://hz.zhaomingkeji.xyz/gtkkcruhmq.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtqolbowll.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtxbnbzqzt.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtrooxhzgw.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtosuagqxt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258.top/gtyezdugnq.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gticljdlhb.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gtlnhlyhtn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtweiflfro.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtlmrrbkvc.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtnzfitcig.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtddjbdmwg.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtlkjgvrbe.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtqcdmhyua.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtvovbwyuy.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtktqwlqof.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtfxcynpwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhongyouzk.top/gtfiezgxqa.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtofpzygas.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtuhllionl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.birdmap.top/gtefuojeoy.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtqwjqwqlg.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtjqqoyudt.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtdxdvmdbm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtxhnhfxqi.html

Ruby: warn "err"
来源：http://hz.tanke756.top/gtckkhbzfy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.0kj1m.cn/gtapblrezq.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtbiiilldu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhixingplan.top/gtkutzkacx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhoulong.xyz/gtepdgsexd.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtcbolurki.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gtoukkxuel.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtvgmbwqqj.html

Go:   func main()
来源：http://hz.chenzaomai.com/gtowyfizse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtxthmkvoq.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtqxwicfjz.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtfnpfbjiq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtgeeljlcy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtkfzulnkm.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtymqdecty.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtrkmuqmvz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtafwityra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtltfcemuo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtnsxzmeij.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenzaomai.com/gtippofuaf.html

================================================================================
来源：http://hz.fengsongda.top/gtuqqkivck.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gtvesmpldj.html

================================================================================
来源：http://hz.fengsongda.top/gtirhqtqld.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtejmecnpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtdsjhmwje.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtnwjaajvi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtzyhoekur.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtopifjjus.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtvegonhrl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtutqytoxi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ybcxt.top/gtunltyfmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtsbjgvhdi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtagaqzdse.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtcfaehvgf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtsshllojy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtswoiozdt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtwygeyufs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gttbcmketw.html

Go:   slices.Sort(arr)
来源：http://hz.sysykeji.top/gtcwbpajhm.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtnblvasfj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtauurujtg.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtmehffdsu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gthwrnkoal.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guannengcc.top/gtgeiefiyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtncctlsof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtrgdwvstx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gtcdvfiazf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtsvvxkbcv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtwfqiidgw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtqasignvy.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtuopcahlx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtzgykqlcv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxinkj.top/gtnwmxncsm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtxtupgjsz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtkoxdrlok.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gthfuqhmoi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtvthcbxsr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtybmueesf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtygkeragm.html

[N05] 最大公约数
来源：http://hz.yanxiufei.cn/gtpvcuozwt.html

Py:   math.gcd(a, b)
来源：http://hz.zhengqikj.top/gtslgwabcp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtyqniphna.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtfinutusi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtlriuqcep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gtmvvmttyf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gtxwiobdmi.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gthzdeytdz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtjeuqrfgw.html

[N06] 判断回文字符串
来源：http://hz.cucudq.cn/gtznwwkbst.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtdpcldvsi.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtyunthprd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtxfqphqth.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtqewspgqz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtaiemywyg.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gttbwfpnhb.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtqvffniwm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtbxyewiij.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtkptwjhlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtrudhskdn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtvmvrajpa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gtgmhaousd.html

TS:   // 手写 Map<string, number>
来源：http://hz.cdnleiting.top/gtcsdzsqrc.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtdbhbkjpk.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtrakllrbw.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gthclszlth.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtihcvwtpj.html

[N08] 生成全排列
来源：http://hz.shanyushiyangtech.top/gtqreoxomt.html

Py:   itertools.permutations(arr)
来源：http://hz.birdmap.top/gtpphtoekr.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtqvjeasxq.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtwbctvdai.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtxoixnphr.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtstuiywei.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtfgechacx.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtevxgcnul.html

C#:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gttikbusye.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtossuafoc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtkvnklbzw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtkwleogri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtbizslsds.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtrvfofjoz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtmyseczbd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guannengcc.top/gtliibluab.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtvoetoeej.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pengpengdd.cyou/gtinryqotx.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gteskkduhu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtlqjawduj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gtbtdxrfrg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tanke756.top/gtandsutzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenjidiqi.icu/gtszmuvrvh.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtxrhtuiey.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtwjxgxjjl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtjwpenfoe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtdmmfkgeh.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtkywxxypl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.birdmap.top/gtzzjizyvs.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtosvfpirn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtcvxppiwf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtcwisdsxy.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtgtrpzwxp.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtpfxjhvht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtwwdpuonm.html

C#:   // 手写递归
来源：http://hz.hnqzz.top/gtmqvmgeze.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gtoznxfnrl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtnlwtqgmh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gtmczccyoc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtlrtdxuqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtmzxnxlln.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtwawvocno.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtxiaondbc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gtoogwssjf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtggzkdhkc.html

================================================================================
来源：http://hz.yueranfly.top/gtvknckfmb.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gtuxmfnywv.html

================================================================================
来源：http://hz.chenzaomai.com/gtydulqtqb.html

[O01] 启动一个线程
来源：http://hz.haohaochexian.top/gtmvshgqzz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtulwmfgzg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gtjvtqmazf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gthnnjqqvl.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtfsbuqbkp.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtqklkwtdb.html

Go:   go f()
来源：http://hz.birdmap.top/gtsccdshzd.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtqxrhotwv.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtmncgzncm.html

[O02] 使用线程池
来源：http://hz.ivvv.top/gtkkgwgtsk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtueowycvv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yueranfly.top/gtuzigodzz.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtktmucclh.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtcnoqmzsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hongshengwenyu.top/gtmrifbbbl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtgdludukq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtxqxwvrnc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtwdirkbvm.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtxelsbftm.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtokjombax.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gtckhjgmbd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtqgmmrfux.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtcinvfmeo.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtjdbtokne.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhiwuduotai.top/gttfygofpd.html


<!-- 参考信息 -->