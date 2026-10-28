代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.tianlin.xyz/gtimytlhml.html

JS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtcvlwldcw.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtfmqnwzhr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shangyingyoupin.top/gtalpqqzyt.html

Go:   strings.Count(s, "a")
来源：http://hz.havefunace.top/gtdfcjxxwq.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtbflxzyye.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtxhhmzqrc.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gtulwqsisr.html

Py:   for ch in s: print(ch)
来源：http://hz.chenjidiqi.icu/gtnngsmwfl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gttqauzsep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtbffiqkxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gttometckz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gtadxstlva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtvreldzch.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtvvxhnyzq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtztiztmfe.html

[E14] URL 编码与 Base64
来源：http://hz.dianchejie.cn/gtbhyyiboe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtkuscjpbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gthejpqmql.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tian-w.cn/gtkzqfkxjz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtwanmqbov.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtinwizxiu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pycfn.com/gteqqrmrbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.iojbl.cn/gtepzhdiyu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gtzfepwcmc.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtrgcwfalk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gtnpmmhatz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gtbowizyug.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtkjnjpbjc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtqethvqzg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangkeji.top/gtetlnyqzi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtypmsmapg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xylfe.cn/gtrsamxmnf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtngculmmm.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtaytvgehy.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtkmurjbib.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtymgawgds.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtuhntfwba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtadcdgdaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yanxiufei.cn/gtsxmjwdok.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cucudq.cn/gtffkjrzxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtfusjjegt.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtcpirmikf.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gtwjelswha.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtesappfqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtayeorrzu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtmdlngest.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtbujiduue.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guannengcc.top/gtwurnuokf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtakqkxuwl.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtedklpkfm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtlrgwbvqf.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtbijrmmex.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yvedp.cn/gtonjlsdnf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtctmkukvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtxwnkyuhz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gttaqoggoa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gtmunskzpv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tanke756.top/gtrbkrzwpm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtxosfpsfi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtrwfbusov.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtghaezdjy.html

Py:   s.splitlines()
来源：http://hz.ehwqpu.com/gtxefkwzxj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtbtxkbqof.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtqwsjadzp.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtlhtbtgrh.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtduklkvyd.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtxvcmbqnp.html

Ruby: s.lines
来源：http://hz.smart0.xyz/gtjwmzugux.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gtexzgjleb.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtkayftyvr.html

Py:   if not s:
来源：http://hz.316326.xyz/gtneyehqwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gttsjqxwtw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtdqocnxzu.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtvtobcuut.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtpzhpbuws.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtkwhxpzhp.html

Ruby: if s.empty?
来源：http://hz.haohaochexian.top/gtzgqjtlzy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtulfhhdmf.html

[E21] 超长截断加省略号
来源：http://hz.9152youxi.cn/gtpufxjaja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtznwljfax.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gthrquctwc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtomglvlsy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtqflqevgl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtnwivnfrv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gtjplwsujf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtsdupblpe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtxktosqdw.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtbinpclfb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtmnvdrcqa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtqldiqkpp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtvokysgjb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtycuujntn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sufxvd.cn/gttytsdtjs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.birdmap.top/gtdttjqtwr.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtxoyffivm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtbxnihyjf.html

================================================================================
来源：http://hz.9152youxi.cn/gtgafmpsbv.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtbvuvexhl.html

================================================================================
来源：http://hz.tanke756.top/gtdrxlpttz.html

[F01] 读取整个文件
来源：http://hz.smart0.xyz/gtwrvvqprz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gtqoyfatdy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gttdkzlhtj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gttiatzghy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gtnwuqpfdn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtnabumptw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtbsqbztkz.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtrcvnsszt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtzihqcumq.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtkzsauglr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtqiwamzmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtvvoelxhi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtrsyyeolq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gthuqlindl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtfmezkzjm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtesqtmlqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtthnxxgyv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.haohaochexian.top/gtfvcehgaa.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtkenzmivt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtooobiwps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yueranfly.top/gtygkwpdmz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtvulhiddv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtfpniwaki.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtkrzmcyyw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtzbqbrtuo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtrndsaxue.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtcidhqgqa.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtpxdjualb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.birdmap.top/gtwlvhalps.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zycfv.cn/gtjwuwbvou.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtywmnuvky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtjfzjtdvi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtmhfvmvgx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhoulong.xyz/gtiijjthzd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtvgnshmpd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtltpigrnx.html

[F05] 判断文件或目录是否存在
来源：http://hz.hysaishi.cn/gtgxbxwsfg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtuyoajgjv.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtisstvzpt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtvdwrhdgn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtgqayyrsl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtdetrjfuy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtcputeyrt.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gtiscjomap.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtnghjgtdu.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtdepndnme.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtghgnfaiv.html

PHP:  unlink("a.txt");
来源：http://hz.tian-w.cn/gtkjgjepum.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtfozourfg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtltvipgjp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtnwllyluz.html

Go:   os.Remove("a.txt")
来源：http://hz.daria6918.cn/gtbeufyazk.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtemmhehes.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtjrtnqvbw.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtwisinjqr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gttvqkpcvp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ppjwa.cn/gtbonyklny.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtclxpnjty.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtvnuwtiyv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtzqfufsrw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtbhevwyjd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nwbrower.top/gtwterkvxq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtuooewrcs.html

[F08] 遍历目录
来源：http://hz.yuxming.cn/gturotsqeh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtqhalrvtw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtyroctqmf.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtznztfogf.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtykfgvvlv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtqcqazumw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gthaismbuc.html

Ruby: Dir.children("dir")
来源：http://hz.ydzc1.top/gtzfodnvko.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtxwhvshhd.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtvqyvifgt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gtmfnkjuzg.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtzhpyioof.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtbkctgtca.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtduwxkhyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtdkqzycbv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gtbobtubtd.html

Ruby: File.size("a.txt")
来源：http://hz.shzxlz.cn/gtmuciuxcy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yanxiufei.cn/gtjelgqkht.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.havefunace.top/gtdljvlvml.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtrtpkaxwh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.bjfxy.top/gtioyyafql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtbmsgfiuu.html

TS:   path.extname("a.txt")
来源：http://hz.cqqwz.cn/gtwglstlsh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xziqi.cn/gtvkajpwio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtxcncngru.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gttoptscke.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ivvv.top/gtckomvgut.html

[F11] 复制与移动文件
来源：http://hz.svipenyu.cn/gtrzyqschb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtnvmuwldm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtrnsqrfkl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtocryxevq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtvxzjahzg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtesflrsuj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtzhqqkbyj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtvmumkdgn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258888.top/gtlwodtnpl.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gtwagbfxfd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtjdmkksso.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhiwuduotai.top/gtkzhggvxg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhongyouzk.top/gttyvinsdj.html

TS:   // 同上
来源：http://hz.daria6918.cn/gthwgkaaat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtxqovedmn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtvxuskqsd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.iojbl.cn/gtaarlevhs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtrcsxuvvg.html

================================================================================
来源：http://hz.guannengcc.top/gtxelgeyjc.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtykqnkvre.html

================================================================================
来源：http://hz.fzhhl.top/gtapbditfz.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtyjlivqef.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtwxevykkc.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtjqoxlynw.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gtkcrhondh.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigfzy.top/gtpcqrcege.html

Java: class User {}
来源：http://hz.52xcode.cn/gtkalaefjl.html

Go:   type User struct { Name string }
来源：http://hz.jyoumei.cn/gticshhtfa.html

Ruby: class User; end
来源：http://hz.yueranfly.top/gteisuiskk.html

C#:   class User {}
来源：http://hz.yonumen.top/gtxmknknqc.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtpxuhktok.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtvdbpwuez.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtvgolkvid.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtkqbdowob.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtjsvwhkth.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtakzjuagm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xziqi.cn/gtfvfyhwrl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtummxctgo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtvzckcwfs.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtiwzvgbgy.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtnhxvypja.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtulvwqett.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gthdbvteex.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtljlymmqh.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtkzpicohw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtveshmnzo.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtwfnzgxnd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtggjsahyk.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtrhinlklm.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtskcavkyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtrqsuxooc.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtpyznqwwr.html

TS:   greet(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtllnueuuh.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtbrygickb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtnimjkmtn.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtdmehomsq.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtlhxnfxmw.html

[G05] 继承
来源：http://hz.gzhubu.top/gtifczcuys.html

Py:   class Admin(User): pass
来源：http://hz.sufxvd.cn/gtlvybicek.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtjzsattob.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtrnlehyev.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtktcejmbu.html

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtgkhennom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtawtdhhov.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtfpusvsre.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtdputidhu.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtgfckuqnx.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gtuhuhlhap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtzloorpdu.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtbdsnxfna.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtftvpjcyo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtuhebvxip.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gthtzjinmk.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtloynuwbw.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtkmlpcmma.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtjnnquxgj.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtljeooxuv.html

PHP:  parent::greet();
来源：http://hz.yuxming.cn/gteukvetqi.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtqjqggzdx.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtukxminxz.html

Java: super.greet();
来源：http://hz.c1oappe.top/gtvfxdpajz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtcnzeehin.html

Ruby: super
来源：http://hz.hywenlv.cn/gtbqmirfpg.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gtlahbxfsq.html

[G08] 静态方法与属性
来源：http://hz.cucudq.cn/gtymigfbod.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtdipvagbl.html

PHP:  public static function f() {}
来源：http://hz.sufxvd.cn/gtwhwuvngs.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtowvbseqb.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtccmbdyoh.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtdiiuymsh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtbxtlapmv.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtwctzxeko.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtkrnjifwp.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtfqbdwgjs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtdqqmaruf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtredbtjrf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtgrxbxaxc.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtwbglfkpr.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gtlzcerljr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtaprezgay.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtruszcryi.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtoeqruxac.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtnbwvbykq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gttjngxovq.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtnnxicwyv.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtsjmqbiti.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtbolwhwxv.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtegyixyci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtzivvjfbu.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtyibynkag.html


<!-- 参考信息 -->