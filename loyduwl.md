代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gorbqhsby.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gqsvmgxuc.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gizlbaatw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/guvxomcis.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gaugbwtxx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gomrtgfko.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gepepymaq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxtiauymq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gbskpnmoe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gapblhkra.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/goevoqooy.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gjicvtoyw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gdbarafpz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/guyaxxypn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkccyrnnz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gpaboqtsf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gmtgtelfa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gvrkzsqzm.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gkkragijr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/guvswickq.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/guouajsuz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/ghmftjkxw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gvcftotwj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gsqrcvhbu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gajuogawv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gfecpinaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbwqqrlfm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gslemcjqe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gaxqyvgah.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gzwmcfmct.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gjbglxvrg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwzzcjxqz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gridrtrfw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gzhltwaeh.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gflrilbam.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gtrxhenyn.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gfllznknp.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ggmvlphgg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gurvswfla.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gyuizhkjp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gqentxhxr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxlcuixmr.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gnzlqwpja.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gqimhxylr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhamrod.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/ghtiwcags.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gpmgfjvxj.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gocfjveic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gnwxkjcpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghxoznazu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmawenufg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwhhhkilg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvycfjp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/giywffjml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjngtdotr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnjehjlbl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gsghgljhy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gsvrzgaif.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gukdrjdsw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glnsepgvq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/glhlrlmdz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/guzduorhm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gdmhripvn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/guyqzwkdd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gvractaag.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnvnrjsgs.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gcrhwicfd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geenzcale.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gsmtxkprr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gubfpklzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/giegyqvob.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gevpdvrin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gdxjxlajo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnwhrbzzg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gztulqekz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkewatgsy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghyxqkbgx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gvljrmahh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gumnoxpkm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gxnyhiyja.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gsvpxerjr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gpzuiwuls.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gepwvmxyg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gerdscnoc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gdsmlmaxb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gjzvupckf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gwfldppon.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gjwnyjsrr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gyowwvqav.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gcjdvrvvb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gbhgpzhyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gyfjebocs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/ghvhkhluf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gmuxmsvzo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/grftmcfoo.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gpljaqjtu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gngbxdhzh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/glpasjynx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghlnaqjyx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gyasnolan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gvnnxvdcy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/ganajwcbl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gwwgwcqmi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gdzbybfeq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gfjtccmft.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gzjbtksyh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsrkehgab.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfjrqdhts.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyvmiixzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxxxjnucb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gbuxytckk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gipwzzmaj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/guevxvczl.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/ggggfmbnz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnnhtoflt.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqxvajdbm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfgukepbx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmeikajpp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gnpaxjxdq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbirlnqcm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdkyemqra.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gyqhootkx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/geaxhdvlr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gjbgtsvmn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gshzjiofb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gzhvyetqh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gwgyfwmyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/goxdtvcxg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/guysuncvz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gfojljbkv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/geghdncua.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gzykwlkzg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gdrbymmib.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gfccpomce.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grxqjusak.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gyileiilb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gfukjopyc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/ghcrfages.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gpxrbwpju.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gwbpedtro.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gsbqfbiim.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcuaryofk.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggglwvzkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gzqfjdpow.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gkzjqfsau.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gplyodwpv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlobjslq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glscqlumd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gwcnoyfqt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/glaxzrkki.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grjslizwf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gecmjbcey.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gejowowya.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/glkegumls.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmlkagv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcwmhqzsd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghwtohzgf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyjmvihtc.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gtwlcvfnp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfmmdrefm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gwzabbwlu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glykjtqzp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghcfsjady.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gcjvtewsz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/guawxskxm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gunlelqnw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gmpuizxsc.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gqehgebsh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ghxctjloz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gtiomqbte.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gjckbyqja.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gwoszpzri.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gzzyosdpb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gpqoyiqah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gqdhkcuks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/ghgihvujr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfdlgimlf.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gwlvizqtd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsdhzrrcb.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/genbbfkuf.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gjhuumfkm.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpqbdmlpb.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gaezwbwqs.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gkyckkijy.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbimzcc.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/guhcpoohp.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/goisbmqfv.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gesnwoovp.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/grnezxlbw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gfunqotre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/golifqmub.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gomgqzcrx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gceqitkxp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gszvqoaue.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/ghzfoasqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gyfjdrjkg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gadelbvrf.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gyvudiirn.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gnohwbdqc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcxftttwo.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwdkofxbt.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gjhjdeivm.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/ghwgvtddw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gddieeryq.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gemkjzfwf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvuhagled.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gjldvadya.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gomrwvklp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gnrrgildt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ghqoxzduz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdndgiyqa.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gnuuetlus.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdjlvjjts.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmanqjcje.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gsbxcvaus.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/goofnifco.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/glqizauwj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnytffshl.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghiwttcos.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpxjlpwvs.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvhypqrlg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gpwdtaqiw.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gddvtvuky.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gdudkvfqd.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gfouseiqn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gzlwqyhsu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqgetmwol.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gijdaqsqv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjnkzlvni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjanurlil.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gqdbyzfob.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gggxwazcq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gzjigjnjf.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gratvecwg.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gceavbtno.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gkgzmlmht.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gojybccgs.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gchfnzcxx.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gjpkbmopp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gwvfwgsgm.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gyxnmentf.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/geyhvxapf.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gtemcqldk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/glirwlmri.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/getwhyhqu.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gknilqyet.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gonlapyil.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gkhttgdfp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gnlfpkgxp.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gxdfkeahd.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gezpzdtkc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gqmywtugs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gpmhezkzc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyjqrlxq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gmrduixhu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/giosfmfqw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gsauomvtb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gjiovojmv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gmslwsdph.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gluyabehc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gpzzvxabu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gxzzhodgh.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbbcmmhcd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gmpjhfzvq.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzbmjupah.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gyiraausn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gmkhmwhap.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjaujgwsp.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gcxbpzjhd.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gbnjvkcne.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gwnevnpio.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gkymmwpbx.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/guwwljzsg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzovutldj.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/glkprofhs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gsdncoccs.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/guykufobb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gywuxfvwg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gozuwtqzp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/ggkxzspnw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glqqmswzl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjarkrhj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmnqwuwza.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdjvbxrxa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzrnxlgae.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gdsqjfjde.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gwfvuddsw.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gljprqxvt.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gdlcehtts.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxgorquao.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grrtyyitn.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnkftjhhi.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqfkrzrzw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gdfuggzfp.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gzdychiba.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gvqjbuxfc.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gvfkvxult.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gaqjzjrnp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gwikdgvnq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gxcjmonhu.sHtML


<!-- 参考信息 -->