代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtffxnixci.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgufenzy.top/gtjmsffyah.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtyylbpson.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtvcpewmum.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtaefobaob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gttbnncklu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gtyykmpxpz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtclrmmixy.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtjshqdfvh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtieohyhxg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtygbxzqdg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gturhyxvhg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtjntmfmxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinyuanbaomall.cn/gtbrxsiwjr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtxuiawhpz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtipenulhn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtdldwjzph.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinghuilouyu.cn/gtruabstuf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtmrxuhpqw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tian-w.cn/gtkqbcliap.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xinyue.icu/gthfgadehk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtomtpsbjc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gthxtvolnp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ppjwa.cn/gtujbcoqto.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtgkcxjlmg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtbyeywkmx.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtgmjrjnfk.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtdkphltqh.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gttuasfdxw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtsbydvail.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gthieekmbm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtvuqsvnrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.svipenyu.cn/gtuyexvcgz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gogol.net.cn/gtcqxceqah.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtooymiqvh.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtmiqrtlfe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258.top/gthzttokhu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtdmxgjshk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtkkbgnkgt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtbyzhpowz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.feifeiyinyue.top/gtwcvottzu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gogol.net.cn/gtvliicokk.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtckbusxbp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtfynxtwpl.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtkcedyzyt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtvgfoxkoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtromddiek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtpnhkxejn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtrwjwxecm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtwzkpyezo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yonumen.top/gtwyoxhenp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtylrmslmt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtwydnjofp.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtsitkwpss.html

Py:   s.splitlines()
来源：http://hz.shangyingyoupin.top/gtidzoeyre.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtifthfftk.html

JS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtrolhwccj.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtqffslojf.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gtmzdpwpbm.html

Go:   strings.Split(s, "\n")
来源：http://hz.jyoumei.cn/gtkyqxedxb.html

Ruby: s.lines
来源：http://hz.havefunace.top/gtosbdawly.html

C#:   s.Split('\n')
来源：http://hz.jyoumei.cn/gtiyttppuq.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtwicwlyyj.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtdetyojhv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtfjytilhs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dashuyun.cn/gtrjyxkqla.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtulgtozao.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtjxlvndjk.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtbjhulzwn.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtdvexlyys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gtrlmbbfxv.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtvgijtopn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtkeionsvx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtegwbmwkl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtguefefug.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtpzppucto.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtwlloswch.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sxryk.cn/gtvnfjvsln.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hfpthk.cn/gteizodouz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigufen.top/gtqtpazyvm.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtjvswvqbe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gtijjknwye.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtcnwiunos.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zycfv.cn/gtjreqnraq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtsnwoptjp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtctljrbqo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtghmbjbhn.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtukslysnr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtirrikhut.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgqskwrab.html

F. 文件与目录
来源：http://hz.hammf.cn/gttvigouje.html

================================================================================
来源：http://hz.ydzc1.top/gtmigbucwq.html

[F01] 读取整个文件
来源：http://hz.jiagoushi.top/gtapfeimbd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yongpay.top/gttmtzvayw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xylfe.cn/gtrbezujvh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hammf.cn/gttlpriyac.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtoynyxrfi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtdnoehucm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtmvxbcagr.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtlaefdvck.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shuidangran.top/gtihwwffee.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtqbmfrypk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtmsuwuocw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtnqgwrtkw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtkoaalkid.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtidsgoipa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtkrylivuh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ppjwa.cn/gtokxcqoyg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtpxwabwid.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gtohnaawdv.html

[F03] 写入文件（覆盖）
来源：http://hz.snrcjt.cn/gtunrbwtty.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aibaodan.cn/gtggsdzixw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtcsmdafaw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtqdommtlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtlaungkqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtfjaogdmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gttsxsjagi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnqzz.top/gtjxhpxhdv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtslgcwugc.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtexcgkaae.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gthmlqpthl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtxdxctvpz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtzzuiqpxe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtjdjriysg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtnfxsdnkr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtoqraezuo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtewjajydc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gttcyxmknu.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtmjhcrmzp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gthkuusxuc.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtjfioerdw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gttyfezlxd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gttfezzutb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtwbkzyktd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtanwqefgx.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtrcunsigr.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gtuvvnhlrk.html

[F06] 删除文件
来源：http://hz.svipenyu.cn/gtiocphhpm.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjwunvwdj.html

PHP:  unlink("a.txt");
来源：http://hz.hnxiangtu.top/gtfqewgbxp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtgfdwwvaq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtgwxaulti.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtfflasbxc.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtundcdeqs.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtjutdjxbx.html

C#:   File.Delete("a.txt");
来源：http://hz.hongshengwenyu.top/gtdqthdcdn.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtaasmhpgu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zdqjudy.top/gtgmdnkhoh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gthtunamoh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtqjuzehyy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtmpzouafm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtlujajlzh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gthtoudhnw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtydgngyiq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtvmrqeuau.html

[F08] 遍历目录
来源：http://hz.xziqi.cn/gtdpqpugit.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxuanxn.top/gtxeozzijq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtoaevovtu.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtqwjiazdq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtbdqmjtsx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtenccspdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtnravrdir.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtezpfejbp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gttococtbt.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gthgpxeevb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtboqggvvf.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtemswjuvs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtlmuitmsh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtnrmqkcyw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtqqbelfzz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtacpudqzd.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtqxecewti.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuanzx.com/gtfqpznjlk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtvofsvalu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gttlweyriz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shuidangran.top/gtfgcpdmep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtasaorgat.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtuqmmwzei.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gtaeqwvnja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtadydhoqr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtavpiwnlk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtfuxrcvnb.html

[F11] 复制与移动文件
来源：http://hz.yueranfly.top/gtngjaewtw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtzveshyej.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtxgwlttxh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtxwnduphg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtrcgrfqhj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cqqwz.cn/gtnznlakig.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtomkmkigz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtbuvzgujw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtbawzlcqo.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gturfjxrnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.redwolf501.top/gtqcwfrvrw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtjaiknqcx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxinkj.top/gtsjixecvq.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtgyrepyye.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtpjbgboaz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gtuwdckspg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtqajggfoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtxsxorjht.html

================================================================================
来源：http://hz.ydzc1.top/gtnpvrpjqe.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtcezuyqko.html

================================================================================
来源：http://hz.xylfe.cn/gtrdtwwtvf.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtbdsljprt.html

Py:   class User: pass
来源：http://hz.shanyushiyangtech.top/gtibpvpftd.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtvuyklonu.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtnetepblg.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxinkj.top/gtmzktgmlf.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtjadxqwxr.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtlhxmjpwq.html

Ruby: class User; end
来源：http://hz.zhoulong.xyz/gtkacmnuhd.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtnsmwukxg.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtatoatufi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hywenlv.cn/gtaagmrdng.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtqkfhesdi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtbnizyuky.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtuxvwplmb.html

Java: User(String name) { this.name = name; }
来源：http://hz.yvedp.cn/gtmposrlcg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtyefeomwp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtalennszg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtqaxkfebf.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gtdqlvnjqb.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtcleosded.html

PHP:  public string $name = "x";
来源：http://hz.sweek.top/gtwfrtelye.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gtfuhwnobs.html

TS:   name: string = "x";
来源：http://hz.ywan-chungtsiang.top/gtysrbxumg.html

Java: private String name;
来源：http://hz.cashguo.top/gtmyshfwky.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtmfxmqasn.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtlixlwnro.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guowangkeji.top/gtolipupgm.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gtohwklvcp.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtxualwelt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtezequeer.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtusrhjibp.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtrxezgyka.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtgbllnemj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtpllpskbq.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtvyoylyjf.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gteyctzwtx.html

[G05] 继承
来源：http://hz.sweek.top/gtyjyddvlb.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtvvkmckck.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtogbypgoj.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtzxsizivw.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gthlwvhzyr.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtxxrqozxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gttmxuxbva.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gtawipxgbr.html

C#:   class Admin : User {}
来源：http://hz.dianchejie.cn/gtdjtivjoh.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtfypyuspy.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtaspdrwxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtkttiuekd.html

JS:   greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtpmrnwddd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtpzefunpv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gthryjfvmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtzqtavmgr.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtbpqsfeno.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtmbhynfxn.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtghjqcgmq.html

Py:   super().greet()
来源：http://hz.316326.xyz/gtlnxttkuv.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtjzkyimcn.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtjvjecmnd.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtywuqbsgu.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtcnngcgol.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtcrlfzerv.html

Ruby: super
来源：http://hz.yongpay.top/gtzpcsgbvh.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtmsldcasr.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtumbdrsax.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtedxmvdzm.html

PHP:  public static function f() {}
来源：http://hz.zhiwuduotai.top/gtgdhwtnru.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtjyhcbyqc.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gtelwyxxdf.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtaynbxtzd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xylfe.cn/gtmligzfkb.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangkeji.top/gtzhqzqxgp.html

C#:   public static void F() {}
来源：http://hz.ywan-chungtsiang.top/gtombmymdf.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtcbonataq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtesbepmca.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtkbjpcxkb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtcieanhcv.html

TS:   interface Shape { area(): number; }
来源：http://hz.mhx1999.top/gtguiwabwd.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtjhexpkwd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtwjqxnuin.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtuopoflnk.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtenqllwax.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtdnjztirj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtbpmzvibh.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtayflqkkr.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gtsabbhqgl.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gthiwbqzsu.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtnttelytj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gthyryjxsb.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtbokgpyam.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtchgotdyz.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtexvsqkgs.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtoxyyyvfz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtqrznwlab.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtfenmgdtb.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtnqlchptd.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gtmcfhdewe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gthrimhjkw.html


<!-- 参考信息 -->