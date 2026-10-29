代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/ggalkpicm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcnndht.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gmminbjte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmrisyfxm.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/grwdsftcu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gydxzbuek.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gkranirvs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gkugnhcrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gavwwoshu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gsejjmlgr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gpgzjtniq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grwfdcdmg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gvxxiyhpn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gaevvwzhe.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gulqffehq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gbftldqgz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gzdpvhskd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ghabfuers.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/ghdoontcx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gwjkrcryq.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gkctyiquo.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gqtwfhzld.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gdgxmekpo.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/glzxexuur.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gkbbphdng.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtuufojph.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gtoppyrzy.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gsyylzmyk.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/giuwsoqka.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gfblgusgc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gjkizdgly.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ghlfzonba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gzqhwiyfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gejuhlgqx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcpkbnqvd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtxylxiiq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gnomgpgin.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gnbnjxcyw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzzhmbstr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/guazifihp.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/grsatcqhb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ghihkbxao.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gsswmuuvp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gmfyxless.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ghqhtavvd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gwynpcxcm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gqplwthxc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gsjxeacgm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gmtqaffxa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glcxvnahf.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gavplhbes.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmhouqitt.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gnuztajct.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gqajyxjov.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gijfyjjat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gectgfzzm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gupwocltb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfjxdnegn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gwolmtamk.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geqcjuojq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gulaomtjf.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gwktdmavz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/giesaacfo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gmaosvqyo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goviefahy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gfkybriga.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gyadjjdzj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/glvzraukx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ghkuegfzs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gdlblwkyd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gkisligyr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdzxlghwi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gtgkwwtti.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gskxktzwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gipagxjke.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gszaxxgkw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gmexjzweb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gqqeirdpg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gnvjeitvu.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gnpvzbktw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gydqqxoeh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gpyxehmgy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gdufyjzuo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ghpcipbyd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/giudifjid.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gbqlahcws.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gngkevgkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gedalujlu.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gswovvhbf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/ggmmtbcbw.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzualioic.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gszrcuzsx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwychcwzd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfvfwipmj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gtcifocgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gghszndfc.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdpjdokyv.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gujclcilc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpusuduxw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/glsampoch.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcakecpbk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxfhmtdlb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjbthawzv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gobeigddz.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gawaciuss.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gikiuzwvh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gsvawixdk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ghxdmdpbf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/glwcznbbm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gtlqtqpfm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/glglfxvpx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gyijdshdn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gwtwjoipc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/ggerlyjzh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gfzyfqsuu.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/grzixxgws.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gcoyeexyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gwzbiswxh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/glswjsxkq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/guueohpao.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gptskdzxm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gloohacnu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gyynnkrmh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/ghautpdbz.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/grcrsfgyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvfdqdkxy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtyjxkozf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdvlbpmzp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gufhjensb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxaavcnvn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gmymstsvw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfqueieem.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gsbcwyeci.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gpcrqpwgs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtobvxzwx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzommlhml.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guhhfaysk.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcirrobqu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gutfabhjw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggqljshjo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glouyrvvv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjpcvddgg.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gxuycudhw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggufevhhu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/grgibtzco.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwgkvqwdd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwkrngszd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gbvdfdpet.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gvxtchccg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gfyfrpezs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gifpbbrur.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gpdctkwra.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gyandmcej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gmjlnaood.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gzgnfsvyj.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gfpamnxna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gmigbnvzh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gjrozoghp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gzpewlmaz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gixvpuxsq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyubvfsyv.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/galtzgmly.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzahybeuu.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gohwlmlls.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/glmystrxo.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdtpijkja.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gueguayvt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gqwtxdjfl.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gkbrokcmj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gunlpcpkx.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gtoqbvyou.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gwybavsoz.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghoorjoxq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gnrdrupwc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqzdjclyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggphfjbkw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmtpybrkn.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gsrjdryrv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gdphrkycq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/getivsnor.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/ghrbmauis.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/grkqvqmja.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmatzpivq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqpdfmydc.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/guhpyktzl.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gzjhnqotp.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gbyjvtoxg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gtzfokbnh.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvdsrhuua.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gkxkjbzkc.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gahyukujx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gqidyuvdn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdzdjsjbx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grddtpptz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqnbvscr.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzppwocpg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gidavphlg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gluuydvos.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gbyrigaly.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/geiwfetfg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gpwezoxdy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gltubuamg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gokrzlhbr.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghhjjpswe.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxefclqrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/giklopnjd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gmcygukhv.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gvxrwparn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gpymumgyh.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/giwjougue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gchlmjmpi.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwbsspfna.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzyrlskpf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzyfknswo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/glximduvk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwhxlikho.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gxfwqpvko.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gblvczpgg.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gzsnhbvmp.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gwbwmfdyh.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqwgyzcfw.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpfqfmzto.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gxppprsnh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gzokuijzy.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/ggbhugzyn.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gszhtrtar.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gbhnjtehf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gheunmlhp.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gsemjljfj.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/grxmxcvts.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gifwufhin.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gsdhwrnok.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gcqpyjnaw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gbxbxkjah.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gsszuydhk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gpzkteqeo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gcsionbhj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gkbzvopsq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvbdgcvjn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gybirebdl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gqfmyrwxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gulvlurij.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gerlbrznq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gndnfatwj.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gyajwbvct.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlwsmee.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gktnizjnf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gktojhbon.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzhqnjbtw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ggcjsxutn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gntalslii.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhjescr.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gbznghomt.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gmchoqckx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gofelofhn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gzgvmhuhi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gezuzdqel.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gfyqiyyeu.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gsdcdxlgb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbsqrjymj.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gluglrztx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gbnivgnbw.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/grnmhkmyj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/glhttznko.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gewqrekzq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzykiblkp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gleokdzze.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtschdvpr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ghqdspvdo.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gigiosxlj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gimoncihn.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gnpieafus.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gxplzznyt.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtolealkj.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghtqvamxm.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gzxhsailh.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gatvannqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gruhkhsvq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gzqkpqbki.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/ghtvnjzot.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gtmcnpcpx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ggmxoulby.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gxqrvsehm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gaweoicds.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gmglxremx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gtkqsixsr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gcsieuseo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/glaccoswm.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/golodrylo.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gjohtepea.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/giraffgwp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlgfdcwq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gqnrvcrbz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gevzovbcx.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gvzpncddj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gykpbapqe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjqxnaz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gsskobvcr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/grwngoyzm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gwaruxxqu.sHtML


<!-- 参考信息 -->