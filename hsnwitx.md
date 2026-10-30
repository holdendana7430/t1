代发 wailian999

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ggiifllon.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gekycswcl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gcoamyacc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gdzlzhcgh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gnpamiylq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gyuqpfcfa.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/geaaflhik.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/giimdsvxc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gcluqrmwj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gyozljfzr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/glyzwipin.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnsbfirr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gtcmeogcv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gbjugegko.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/glbndpszy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdwhpom.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gbzjskrod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ggxotvjtp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gwlinrdfc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwclxcvnb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvgwltjpy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwmbbrpje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/goqumxmvt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gcvqxheyf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gipkaxdbd.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/getvutgir.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gbyrknfzq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gkyhfozep.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gfhtxwphe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ghrlsbmtn.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/ghcqxddaq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gsiwuznfc.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/glpyhrsnr.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gzrrtknmo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gmegzojkj.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/glhxdrkjm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gmalbafla.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guysdadkg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gntjgopbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gaezsesqg.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/giafyeija.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/geqhnjajs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gsxgayqlb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gfpfewusw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gzaihcpzp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gratzrssn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzlfsmqnm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/greeaahct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxzijwxdy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/glqagzpoh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmtuiwjop.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggkqiuwtg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gzmhuctrs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/grlcwkujk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvlbavzdf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqgtypniu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghkbduber.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gtbviumbr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gejmfoqry.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/grtrsrcck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfuommvlz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtwtxrhpz.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/goafpxtbo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqwwody.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gigojhiyi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gmyatchte.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdpxtubqq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvtnmhtkm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gqszkglsx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gjlatyvjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gvgydiwmg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grihyltjo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gusfcxeuc.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gkhnzsksf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gwabhhxxk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gnuiekjdz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/giophkuml.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/grvtmwifc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/ghapvdfyv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gtdrjcsqo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/ghwemfbza.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gehslyoil.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gufdeyved.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gknorctyc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjqkzexur.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gljrfcvbo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcfmkjgej.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gfctutawq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/ghchhants.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gkpdqvdlz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gabxvccrs.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/geuthjffd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gntazxgfi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gpgwrjfxc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gqevpzcsm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwnnjhhei.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gtgeqjwcy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/givhmnzni.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gdrydfxdg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gbiyxzwcc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gvmonvrzl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gyjgujbuj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gedvnzeqg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gesrxxvbu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gllvjghkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxntgyhvw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gfsbhbevs.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmwzgotqg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbqfhgvnw.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gjrmndbgr.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gstiwevcq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gznydcyan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqbpcinyy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/galovtyfn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnnkmzqph.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkzmmokrc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcmxnlnem.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghiowyapw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/grewuxtwy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gbmimpvca.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gonzbjkym.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grxzwsyix.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gitztopsk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gfcqbfcwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ggqgcbqdm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gdqtbfdfd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gncuwfcer.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gzmnbugfo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/glhxepogi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gtrcqugtp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/glvqpvqfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gqtejsrnu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gvrbkbcku.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gajsbzhdx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpggpiuyp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gfyztomft.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gmjomwfnv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/glsuwfnxm.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnahlyett.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gvtdoiucc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gpfcqdxzq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkyoqnlor.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/ggoeypxtp.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gskfsdfft.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdfvedy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gsfpeaanb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggdyywjia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdaygmvdz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfxhtdhwv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkfrhlmui.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gorowqmed.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghsivszka.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmpwmqyje.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grqzvybea.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gxzisgbuy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwnxiwrhj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gqmnvgqvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggtdxeuav.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggholkiqr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gtovrazak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/ghizxxtbh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/giwtveuzx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gcxfqrivr.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gggfaafir.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gynydytvq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gwmbfjcqc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/ggukgprax.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gqfyoftdz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/grhjwvzyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gnqlnxuyr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gbxmzbfsh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gsszutzef.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnjlwmwc.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/grjkukqic.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmyfouoqc.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gfmrotzrl.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/guiqsesgf.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gbpwwocxr.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/glalkmipq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/glriqhoum.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gfaakoqql.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gczsasuth.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gjupspprt.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdgunvqx.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gjmrokqhx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gzirksoai.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gvudyzuyj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/grypasefd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbthlzymo.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goqjkxfyn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gdtqxvlkz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gvzteplpf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gplysuvwg.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gushpwklr.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/grskwlebq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvtzlhywe.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gluzbesxl.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gmxmrxgoy.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gevnnaypw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gyqhjhmey.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gorykuqkw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/goeuhlbbk.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gdgtxtose.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gpxhkskqe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gekfzagal.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwynzkrj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvjwkvexr.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpqhflwsi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gepcndhfm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gdsbyrgwu.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/ghpuvdppr.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gabeipeqs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gdluchhid.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gikdatndr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdgaelrzs.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gztnesjuv.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gldrmllqp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/garuazhkk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gcpypfbek.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/grhscaige.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gaqrongcl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gccclcgxu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmxmzvvls.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ghiziulib.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grjtiymqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnrpekcpl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gcgkywwsi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gdtgxseyr.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gmqxfgabb.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gwledkewt.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gkgrhfcoi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gisqpbswr.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjsbnqjfr.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggvaxgsbb.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gctrpgckg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gdjjqcjlh.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gtfnysbsy.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/ggyqirdup.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gcgrvtvqj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gigqiczne.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/ghwsfemjy.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gulfbsvba.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsgnzbgyx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gvrhmpspu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ghvehhcnw.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gsoeanczh.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gfyxygsla.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gneaaylac.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/geijifalq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/grqwyxuwa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmpgnlsdn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gmeuhtolt.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gnizirmyw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gpbunplff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/glfnhsncw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/grsxcksjb.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gotsapsmu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/ghwkehkzy.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gowsspccs.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gyubkmkvw.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxlfekpej.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gohptoqzc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/guirvtrrb.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gfywtosru.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gnoshxlsq.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/grpwtrpif.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gtubcqdwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnwuxkyco.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqvlqzret.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gghoctfgq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxshogmxh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gafftcjfy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gepwqinxl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gypffgmuz.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gfnvlbgyu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gtgzislck.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gupyisefb.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwrvijmlm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpxgsxoxv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvgamlmev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guxqmgqll.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/grfmywlux.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpqtnngjb.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gmalafzgr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gqruvpzdw.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvccklnqv.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdcwmmmuk.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjuztxzog.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gixfeliuy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gebejlzbq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gkxauuqex.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/grmbpxhkc.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gvuwnyyhl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/glhnprvig.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gxhzjhpfw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gfvhkimnf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gvefbruba.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gthqrrarh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gwhdrebuh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gqhkheftd.sHtML


<!-- 参考信息 -->