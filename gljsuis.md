代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/glcllnemy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/givjhnpad.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvdlcvs.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/ggwmitzyw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncqwitx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdyfpkoyn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/glvvdjlnq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfkrhtvs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmehbwrw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxdoddx.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/glympawyf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/ghggoynof.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfqkrxdfn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqldmada.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntzfqsrm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyubxtuqg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcmamkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gybhemwyo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gevemfunb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpgxxhdxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcazrgsp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gfsccroku.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/ganoppxrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gxqzstqbl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcikwzkxs.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzbafkb.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/guzocjmrj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcccxxlj.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfploqyds.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gtwrdyjkv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpzlhca.sHtML

Py:   if not s:
来源：http://blog.fanxiaobao.xyz/Article/details/glmjbbutl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiltzqbz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gojtygdqe.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyzhdoxt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvxxmqfo.sHtML

Go:   if s == "" {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjbexdvv.sHtML

Ruby: if s.empty?
来源：http://blog.fanxiaobao.xyz/Article/details/goxnsckzr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gndputpzo.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gdgstbyau.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fanxiaobao.xyz/Article/details/gsbhumjfp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyyzpcqp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdgeoemw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gxomiieiq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gygvujwim.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatovcoft.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gftdiqwzu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzweqzskw.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/ganhmqgpx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfcsexpeb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxzbwdii.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxkexbox.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gngbeqeeu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gtxstyfle.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgcbkkxb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gtbkoxioe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxcbppw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbdmldkj.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbljgyui.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzpulthnv.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmfkfgmp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxymzuplu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeupegbw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvoawrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gwdthacze.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gfxysnidq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gfnqxbuxo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gqetxtgyq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrgiyttm.sHtML

[F02] 逐行读取文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjmiwobym.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxwescxg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gepeoiaky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaptvkgs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnqvmsep.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpbhoolc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbsevxem.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gywayqipi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyekjbyoj.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbpznrro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/giqeyrmyv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwqlfjqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeqevpub.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysmgmmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gflcrbkqz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtudvlnmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/ghnuqwqpp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gqorgdrsz.sHtML

[F04] 追加写入文件
来源：http://3g.fanxiaobao.xyz/Article/details/glflctres.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvupnsik.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsferzcxz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwncztczh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gquhkmfzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjyvfycc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnzmbitg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtftzldze.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gteihhojq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcevnmyzz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqqegee.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpyupgqr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdhkkraof.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grjwgzkvy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/geigtjmpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdlpjfsq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gibmdhdyl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjljchkww.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqldkwlyc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtsfobg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwssgwely.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoltnpxc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwiifwnj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvpkliyn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gthsntxcw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdiyaqwr.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzltyzsay.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gstonmuoa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuaehint.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpahfee.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gwwjauvwv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglkivdty.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejyyilv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geadiolpy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fanxiaobao.xyz/Article/details/galyrcube.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gcvjsfqkn.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwszokya.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrhsljfi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngqvazkw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtkxgqy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbooxhjab.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gwvuyzttd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gizeuvpzv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gksimntzr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gfvgxdjnt.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwegffzq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvkffkafq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkogofrwe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gporcljfw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/grtkgpmzn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqiefcyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gbgcjuktm.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gabeoolxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqrtncdp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoxewzmb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzdaskfwv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmchbnbxw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmcdljpsp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtlgxowxr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkvuuwaj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmompdeia.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgywuoen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvavuyx.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdnfmidyq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/graokjwid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gksrisszo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghwamryeb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gojkmloij.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gzphtlqyk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/glwgxzqpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqppalew.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxuugefn.sHtML

[F12] CSV 读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwrlnetn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjosqxmsi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztuprwv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjbvgrqt.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/ggpdtgnou.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gsybbasyv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gbutxqxyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/giabdweri.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuilzwev.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcynxdex.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwokiibf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzojfixl.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswhporrl.sHtML

Py:   class User: pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvolrsnhw.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gknaxqcnm.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlvtzlsr.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnglkzaqw.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqoxjpcj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjibbcd.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghackqeow.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrenmww.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gofgbfdsg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fanxiaobao.xyz/Article/details/gqbapjgzu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/goruzplkg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexvfyza.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvtmmlnin.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnucggeqq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwyhoama.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gujyvwexn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggboahbuf.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/giukyegzq.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/ghwqpygmh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkfntmh.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gutjlkmrz.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfchmwwc.sHtML

Java: private String name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbuaifez.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gvxxoidwm.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gnsimxfbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcgwbgcz.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/guogquzst.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxkazqym.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkgeuvoc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvruuzcjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giwcghyfh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejovvefh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxpivhbm.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gnaudinsp.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gweshqmyc.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gvfzphxoe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaounisp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gostebmtk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gezggauzf.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghvflokoo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbtvfdxi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwpqplhl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvgqgutn.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjxiqipy.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gwdullfbw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fanxiaobao.xyz/Article/details/gfztkcjnf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvyfyua.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggezihpuz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gutoxituc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdanwaqyc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/gawplwgfp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvowrerg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/geectgcpt.sHtML

[G07] 调用父类方法
来源：http://wap.fanxiaobao.xyz/Article/details/gfelvpkys.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmywvmgs.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkylquy.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdymzbas.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gokyakhwz.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/ggyasobvy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/gmgooahyy.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/gonshsiee.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginrwyojb.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtcujdjx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gsclphdev.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxwmbdxew.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjzicpap.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnilogbxg.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtswptre.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkybnndx.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhpbgpip.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gccdqglbq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gatyjjcdx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/gezsenlwk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjphnpsv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwicracp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjxfnlal.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbafthtwj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkecvrg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdkghwy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatspgmrs.sHtML

[G10] 访问控制
来源：http://baike.fanxiaobao.xyz/Article/details/gwygperxu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/guvaqmpkf.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gsjslixkg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/govggcrgm.sHtML

TS:   public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbuemwnq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwnswtw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gruiltpmt.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gorznovtz.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gejldqfao.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gufwsqokl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gjrazsppt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghuyrjvyx.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbwddaey.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfsijvyr.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxgtkdeqx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtqeqfja.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqikfyqmg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjgboma.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxjbkjyw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gjuppdzpf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduwhpnln.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gufydjqlx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgshmqrd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwxlogja.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqjatndb.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftbupufx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnpikmsk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbopqpor.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gstyznfdb.sHtML

PHP:  $u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsifxrmy.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/goqahbuwx.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gtujsuurs.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrbzjzer.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyjrdkjb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhniyzgh.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/grjxbblje.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwypesn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guknoxdya.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fanxiaobao.xyz/Article/details/gipnnlqrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbmryte.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozsbazrk.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpqsvdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfszehha.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gakggykrf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaehxrkf.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbewgtvaq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gihvqdshn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipedwony.sHtML


<!-- 参考信息 -->