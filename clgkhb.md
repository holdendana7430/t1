代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtxuidiefd.html

[E15] HTML 转义 / 反转义
来源：http://hz.vqdsnc.cn/gtunqvtuas.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtnpaahbze.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtoltrfesz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtrfnwnauo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtepyzvkeh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtucobdprx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gtlxurghdy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtezqdsqnb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xziqi.cn/gturyycfcb.html

[E16] 数字千分位
来源：http://hz.pengpengdd.cyou/gtowijmibh.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtopgdtlpm.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtzshnuwbx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtgudqpkmo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtdbezxrzz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtaihdotzl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shangyingyoupin.top/gtmhkvksdz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fzhhl.top/gtyhsuychl.html

C#:   1234567.ToString("N0")
来源：http://hz.havefunace.top/gtdbuhxiln.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtesisthaa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtuveqwkyc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtwzgmplth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtlhqekpyn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtrswtakte.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtjoqjqkob.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.smart0.xyz/gtxxqlnspw.html

Ruby: s.capitalize
来源：http://hz.dashuyun.cn/gtgncdoxaq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtbcvyvmcw.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtcwlxkfsi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtrxwlqdbi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xingfuxueyuan.xyz/gtcvwxesvn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtmsorhxjh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtynvhvkqb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gaohongyu789.top/gttczswpzg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gteemzowpr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtevgxsrwv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtjuojhwyj.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtmfvkuytw.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtlunrkzeq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtcmsoxsiv.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtiwfkyzbz.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtrnekbkyc.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gtgoencskz.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtaicqeuyq.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtxtkosuiy.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtccgiaqse.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtjhsedvcw.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtyazplkmi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dianchejie.cn/gtapyqvtdl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtsjozlzxb.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtxzonmddq.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtajuuturr.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtsmocphwd.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtjcvpeudo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtblrzvsto.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtkxduvczz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtrbiegldy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtkvbllgnq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtihfpybkt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtoneoiviy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtkoihmlof.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtxubnrbpp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gtouqwhvql.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtjgpxulhj.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtmdvqcuxv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtfeahzjdb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtmjmzfjrd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtjjdenoyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtljobvryd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtxubzjnim.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtsftprjkv.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinyuanbaomall.cn/gtunhzhqpe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cheryme.top/gtncaontzg.html

================================================================================
来源：http://hz.9152youxi.cn/gtnqqetgbj.html

F. 文件与目录
来源：http://hz.hammf.cn/gtmontozpu.html

================================================================================
来源：http://hz.fzhhl.top/gtxmrkpsqj.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtcizvdfzn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtuyirfybt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtsbhtzdgp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtlgrfghmx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtlpnmvtih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gttybzfkij.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtehlszswq.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gtkkakfbgf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtcudbelho.html

[F02] 逐行读取文件
来源：http://hz.ppjwa.cn/gtxwxuvbqk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtbxexcfxc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtjtdymgtl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtdjtwhfpj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtegivalzu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtmhxtdcmn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtxijulpst.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtpupslbsa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.iojbl.cn/gtkityahmk.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtfpuvkfvc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtmcxinrdh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtysvllzwp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtbtwxisrn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtptptfkdk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhixingplan.top/gtsfccqsae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtdgdaywmx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtlnkfxppv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtaojuqatz.html

[F04] 追加写入文件
来源：http://hz.tianlin.xyz/gtbcilquls.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtxrryeowc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtnfhtcnef.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtthotxoqj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtyhaocdgh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtjhxgobxq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtktnciloq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtlvrpkmfg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtcltfnnlw.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtyviwnxga.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtkqepobbg.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgfzy.top/gtextgepbf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtkrveuqpx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtxbamtiip.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtrcwfkxfl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xziqi.cn/gtljtipuex.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtsslngxic.html

C#:   File.Exists("a.txt")
来源：http://hz.wangdashe.top/gtjizocznt.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtfspxhdob.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtbrimlmal.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtprmqbqmk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtrfzlebbp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtswxwgzww.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtitmmadqc.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtcvcnlaoz.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtgqhdzodx.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtsuvpopxm.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtqwuddzjv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gteroztsis.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yueranfly.top/gtpxdwyqyp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtyjuzycwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtufqnbsjt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhoulong.xyz/gtiwbicdrx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.bjfxy.top/gtoqlsjcbd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtdncsimne.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtwhdsovwi.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtcprbfbgx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtiwhvukim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gtyyvodwcr.html

JS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtxrfyuglw.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtmxtkexjq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtautjegbh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtvakwkjqw.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gtmhhtrmya.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gtaupgleob.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gtckrmcsht.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtnhxmipct.html

PHP:  filesize("a.txt");
来源：http://hz.sysykeji.top/gtrbbdaiml.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtdphvseai.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtgynanlyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtytngzifc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtdcqmkvmk.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtltbjsioz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtbetlwcxb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtgfcmrsds.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtnyffznle.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtmabnxrzn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtrzmxbokg.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtspmtkntm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtsgsykolg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.c1oappe.top/gtjcgblaan.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtwyrgrjgw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtepnyhete.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtlnhjgber.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtjpfvtmvr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtghzidwov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtwfucruph.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gteyasolqg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gthbklwtkd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shangyingyoupin.top/gtsriuasoa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtbwkihthm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtecmvzayo.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtisqgpcrt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtwzieawib.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ybcxt.top/gtlahdtzxo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shuidangran.top/gtkyhfqpkc.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtyseuiceh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtkmbfqiis.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtlomljgcn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gtqicxktgl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtwdivfbyi.html

================================================================================
来源：http://hz.tanke756.top/gtjnothyzb.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gtmkbeitpr.html

================================================================================
来源：http://hz.birdmap.top/gtvlkuyxcq.html

[G01] 定义类
来源：http://hz.nanxuanxn.top/gthuggcoiv.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gteikqdoma.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtdtuxehoj.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtcqwntqlj.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangkeji.top/gtllveoesx.html

Java: class User {}
来源：http://hz.jinqigfzy.top/gtqrwqyiey.html

Go:   type User struct { Name string }
来源：http://hz.zhongyouzk.top/gtkkiyxvlm.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtqsijqelm.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtikpecnyw.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtyzyamdfg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtqyiyhfyl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydzc1.top/gtxmzjkeys.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtpsgfshmy.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtuzytdoqt.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtzezodeqr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtfdtecewf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtqcrbhgro.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenzaomai.com/gtrhlzlgme.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gtjzbebufg.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtyajvuwmo.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gthbsbfovt.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtjdmpxske.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtqeaikwte.html

Java: private String name;
来源：http://hz.haohaochexian.top/gtnduvrfzd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtcqtigmzv.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtchgybmwg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtypjqqfgs.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtrthtqinc.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtaeeaciki.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtncxgheob.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtxwvvezic.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtnikrcnea.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtnsizhovc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtabvoedmi.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtuwigmnee.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtoppyegko.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtevnhqyix.html

Py:   class Admin(User): pass
来源：http://hz.zhaomingkeji.xyz/gthablwhnh.html

PHP:  class Admin extends User {}
来源：http://hz.yvedp.cn/gtmpzeyyrz.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtdyvqpnjl.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtnlqjchkt.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtojkdqglk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhijiandao.cn/gtlvthxrqm.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gtcaqvynyz.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtavxdqxpl.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtqrvsdfkt.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtscgjewso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtlyudfiyb.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtfikndvns.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtojykftgs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtublujitn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtohvolosb.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtdyxkqtvp.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtbvhvspxo.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gttiwajmar.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gttnlnqoqs.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtsuwvwqsp.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtzozersvb.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gtgwiljytw.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtrjrjspva.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gtuqazjejr.html

Ruby: super
来源：http://hz.yuxming.cn/gtsfwhakga.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtjqsjjeyu.html

[G08] 静态方法与属性
来源：http://hz.zycfv.cn/gtxnjxfeyd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtquwvmcev.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtvmuoipbi.html

JS:   static f() {}
来源：http://hz.sweek.top/gtqviuxyad.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtkculckck.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtlsfnrcer.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtziexrmit.html

Ruby: def self.f; end
来源：http://hz.yuxming.cn/gtoisydxtq.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gthbtyoegb.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtzbzrztjx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gthmdbkveo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtoxkrnmio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gtmvlmkunh.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtyunrnhdg.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtxajdqfft.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtoqdficjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtrngdtijr.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtgxlaocpy.html

[G10] 访问控制
来源：http://hz.ehwqpu.com/gtaqacvdjk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtvcvzdnnm.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtabtvbsly.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gttqqucbpr.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gttwvoglfh.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtrbutilij.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtpohkddwq.html

Ruby: public / protected / private
来源：http://hz.ppjwa.cn/gtjdrvnhxf.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtlxaagnvc.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtrzkupjfr.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtojdbgvzd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtbaexrycp.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtozwkfbif.html

TS:   get name(): string { return this._name; }
来源：http://hz.cdnleiting.top/gthkkhplcu.html

Java: public String getName() { return name; }
来源：http://hz.hnqzz.top/gtuecvsffx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtjxhnnfgt.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtoittuczo.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtrexaybjq.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtxkocypzr.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtoylrxkdf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtxazkfuvz.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtoibfytxq.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtwrjiaqik.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtdybuhjle.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtrixrwsps.html

Ruby: def to_s; @name; end
来源：http://hz.fzhhl.top/gttzvcghso.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtjsvwyhxr.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtvagndhoc.html

Py:   isinstance(u, User)
来源：http://hz.daria6918.cn/gthjdgiodd.html

PHP:  $u instanceof User
来源：http://hz.daria6918.cn/gtgbpvnnqt.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtciyaakxc.html

TS:   u instanceof User
来源：http://hz.snrcjt.cn/gtkbaqqpfl.html


<!-- 参考信息 -->