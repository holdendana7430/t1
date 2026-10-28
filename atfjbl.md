代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtxrimsdqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtrdybtvyn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtuyfpjsny.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtnqpxsvkm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtoboidwte.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj202588.top/gtpaizwkhl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gterfbgjat.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtuziooevj.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtsmicbdaa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258.top/gtsmmftqfk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xinyue.icu/gtchepktcy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.0kj1m.cn/gtmlaijexp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gteftkzvjn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gthbylcyyk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gtnsgdxlvr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtrablhaad.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jlsjyb.cn/gtckgmpghp.html

[E15] HTML 转义 / 反转义
来源：http://hz.ehwqpu.com/gtivhetoqe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtvtcyeyvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jianghu66.top/gtnyyvbwlw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tianlin.xyz/gtkxlkgsyu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangtech.top/gthnczizjh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxuanxn.top/gtahingmqq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xinyue.icu/gthczyowei.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtzmtaiogm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtyvkxopia.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtrsuczucu.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gthkcvbwbr.html

PHP:  number_format(1234567);
来源：http://hz.zhoulong.xyz/gtykrjlgmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtfftvrvde.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtmxgvmndf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhoulong.xyz/gtutleofuh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gtbsdlnjab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xinyue.icu/gtvzshvgbi.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gthqircdym.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtxkzfbqgb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtyvclntkk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtbfzjmjxy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtppzwfmps.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtmllialow.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtgcodiphy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gtorgqmfsx.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gtqlogczyp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtxaptpkrg.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtrxxfqqbt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtrkbqgiya.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtrsqcjsko.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtjfguekvb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtvhvvgzhn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtgokeqglc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pycfn.com/gtxvpeqeei.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yonumen.top/gtpiqihfga.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtdttrdfhq.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtnjibrdmi.html

Py:   s.splitlines()
来源：http://hz.daria6918.cn/gtppoovuco.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtdvrhmuje.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtssrhzeyj.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtvfvopacj.html

Java: s.lines().toList()
来源：http://hz.sysykeji.top/gtbbfkmciq.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtsjojifwj.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtnvytipoj.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtxkanjufz.html

[E20] 判断字符串是否为空
来源：http://hz.xuetiantiany.cn/gtydvudxsr.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtyfeqnran.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtegboqezi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtyqeuqpqo.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtrpvvniwc.html

Java: if (s.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtieegpavt.html

Go:   if s == "" {}
来源：http://hz.yj20258888.top/gttxhpkgoh.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtatrtebvh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtwqkujzjc.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtibxvqdpp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sweek.top/gtumlsomlu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtjjlyuprf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtibdbocze.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtuvmooyqc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtcubtquoj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnxiangtu.top/gtqxsnepds.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yangfankeji.com/gttlspuswu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuanzhike.top/gtbsghnhhd.html

[E22] 字节长度与字符长度
来源：http://hz.jqgfzy.top/gtlmxphbyt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtfmmlwgxe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gthxxynyim.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtmeigwbkq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtchyiaijd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtzgfnwnng.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtsykqjyeg.html

Ruby: s.bytesize;  s.length
来源：http://hz.yonumen.top/gtipbmlryg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gtioknlqad.html

================================================================================
来源：http://hz.wangdashe.top/gtzkjafrvm.html

F. 文件与目录
来源：http://hz.jinghuilouyu.cn/gtqpgukacx.html

================================================================================
来源：http://hz.sxryk.cn/gtbdxujrhk.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtvoerqvou.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gterkbbngz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtiwruyibj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sxryk.cn/gtcjvmtiik.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtvqlypbgr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtrtnnmxkv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.svipenyu.cn/gtsaeifnle.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gthwurtdje.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtktyocopk.html

[F02] 逐行读取文件
来源：http://hz.redwolf501.top/gtlzixdcan.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gtocwapkdg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtndysxxsj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtlsmhrhpf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtobarvghk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtcgkxbrqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtyzfvdagi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtfisgphcn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gtevakfued.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtgtmxytzd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtgoammons.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gthufwlgqn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtgqmcoeia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtkulbabvi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtgjzoxlqo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtpbcuplux.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yonumen.top/gtjvoznblb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gthlpmsinv.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtvaunfaoj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtlynydoto.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtheykcavy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtzznbakrv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtffgbwlpt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtaughogwq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtaokjwzlh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cashguo.top/gtlzelnnbf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtxlkiiaiz.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtdxtqphiu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxuanxn.top/gtdjcfbzgf.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtlhglltsu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtbkfozbhj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtlmrluqmo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtpvdgxnru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gteyexwrok.html

Ruby: File.exist?("a.txt")
来源：http://hz.xylfe.cn/gtupybkila.html

C#:   File.Exists("a.txt")
来源：http://hz.yuxming.cn/gtpmpiaiej.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtfknawpfr.html

Py:   os.remove("a.txt")
来源：http://hz.daxiang520.top/gtrgktwmyl.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtmnextxxg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtbcyzigxx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtknxmiknn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtufccbnoh.html

Go:   os.Remove("a.txt")
来源：http://hz.yuanzhike.top/gtmqrqkwdm.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gtpdtnjbhk.html

C#:   File.Delete("a.txt");
来源：http://hz.fengsongda.top/gtkfeiinky.html

[F07] 创建目录（含多级）
来源：http://hz.kuanghao11.cn/gtjsdevyus.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zycfv.cn/gtkbxoayge.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtqwvzvsgp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtmkpfpuyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtuilttzzu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nwbrower.top/gtgmzxqtcs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yanxiufei.cn/gtvfuowies.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjfxy.top/gtgbcxuxjh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtadojynqo.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtqrbcznsq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtnnrqsnim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtzjgqdaye.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtihyheupz.html

TS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtqjasbcls.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtvsntteyq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangtech.top/gtyitzgqrk.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtzayytscv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtjshmgplj.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gtgwbtghzd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtbqbwzdus.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtoagrhley.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gticqabmnk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtbhworykb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtqzokbdyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtvekeptfx.html

Ruby: File.size("a.txt")
来源：http://hz.jianghu66.top/gtzjioyrnt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtwyvgvbcl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gthcqcrmbn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtqincjcci.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtnpfbroba.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtyooanfws.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtwmhciauk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtpymtsykq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtxhsuoexu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtwpadkkmt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtrrvkqavq.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtituxmrny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtzrqxomhm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.birdmap.top/gtfuarboul.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtkskiqiso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtjjhngmnl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtumkamnja.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtmvubwyza.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtrysbctud.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtogcuthoj.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gthnfppqpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhoulong.xyz/gttzhcjkge.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtllsrozla.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ehwqpu.com/gtvuwzpjix.html

TS:   // 同上
来源：http://hz.vqdsnc.cn/gtkwyqmyxf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtycyceucx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtphzwcmfe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gttbdhrglm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtnswvlqxt.html

================================================================================
来源：http://hz.cucudq.cn/gtyqjddrgf.html

G. 面向对象
来源：http://hz.guannengcc.top/gtdczaqeqg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlvqepslb.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtzohzkger.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtnfqacgnw.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtqgqdeeeu.html

JS:   class User {}
来源：http://hz.fzhhl.top/gtekdvzyyk.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gturvuzcvk.html

Java: class User {}
来源：http://hz.sxryk.cn/gtqyiytncw.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtzifyimfc.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtqnppdtjp.html

C#:   class User {}
来源：http://hz.yongpay.top/gtixwoxoni.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtbjkomghc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtichdqtan.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dashuyun.cn/gtgbuhnunb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtwdruyeja.html

TS:   constructor(public name: string) {}
来源：http://hz.jinghuilouyu.cn/gtqvitktyc.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtzgcngzjr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtothiueel.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtpawlbhug.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtjcxzqlxw.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtmgltyfxg.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtvhewtyrj.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gttfsfwmeu.html

JS:   this.name = "x";
来源：http://hz.jyoumei.cn/gtgwkvayxa.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gthyicprvx.html

Java: private String name;
来源：http://hz.yvedp.cn/gtkqgeodym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtelrjwoee.html

Ruby: @name = "x"
来源：http://hz.cashguo.top/gtlowvavde.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtsuaocybg.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtjyumgypc.html

Py:   def greet(self): return self.name
来源：http://hz.xuanzx.com/gtymsfrsfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtwfhzdktf.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gtmmbkcgug.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtsbjbnxfz.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtxpdanemm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtfjvvttbo.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtahponlga.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtvhvgmdlm.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtrvkblojj.html

Py:   class Admin(User): pass
来源：http://hz.wangdashe.top/gthrxilcyz.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtjnfrrwye.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtdghenkmf.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtbuajbrao.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtjkjbtxkx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtjnavjclv.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gtllkmdxts.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtysnjnlwa.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gttteumzrn.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtapevnstj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtbjioeijm.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtcnljtcqc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtsurjlely.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtwymmweba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtowxmenfs.html

Ruby: def greet; "admin"; end
来源：http://hz.gaohongyu789.top/gtffrrivih.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtvekhwtlq.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtaytbifik.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtrszrxlgv.html

PHP:  parent::greet();
来源：http://hz.wangdashe.top/gtnwiuvvjr.html

JS:   super.greet();
来源：http://hz.ybcxt.top/gttnwfopft.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtaribhasn.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtslpyxazb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtmhdlwwnr.html

Ruby: super
来源：http://hz.tian-w.cn/gtjxaequzj.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtqqfnehjg.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtkaqrdpjo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fengsongda.top/gtzorlyqyk.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtyhhebfmi.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtdeydkkal.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtdevhqird.html

Java: static void f() {}
来源：http://hz.xylfe.cn/gtwqjoggxb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtctkfaqlp.html

Ruby: def self.f; end
来源：http://hz.redwolf501.top/gtslemyzbh.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtnccanyhs.html

[G09] 接口 / 抽象类
来源：http://hz.svipenyu.cn/gtmlulbunh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daxiang520.top/gtauuntgei.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.iojbl.cn/gtymxazadj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtqhpusavu.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gteytzdrag.html

Java: interface Shape { double area(); }
来源：http://hz.tanke756.top/gtcbsqlpjl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtlssthhvn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtqihwzwpo.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtknvqbrra.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtlhxvipzx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fengsongda.top/gtttdofrux.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtagccmuum.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtumbzfnda.html

TS:   public / protected / private
来源：http://hz.jlsjyb.cn/gtqlxixzyq.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtpgupnezt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtkcvhpzxi.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtekwvqqrq.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtsdmzyece.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtmrlhmbca.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtpoegpcrw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtkwdzeujt.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtwnldwndk.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydjk.org.cn/gtureltfhk.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtobmypuox.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtctoeyxnp.html


<!-- 参考信息 -->