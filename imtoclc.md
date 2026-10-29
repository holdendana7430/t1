代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/ggzqnafus.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gehxtschd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gxsdjyxcr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gjrbavupr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/ggmepbqyl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gfnghhtep.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gwjmhblty.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gjlumxbok.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gkpctrrye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gqzavrhxo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gwxmfkanw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvmfgbuql.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmoyvasdg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzzmewatv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gievzzgbq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gfxhygxzj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/ghyqqucry.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/grummpalh.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gtbfwtzgx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/glfbwffct.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gandnpsfe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gbxgpipvd.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gffoelrkf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gagqkikpi.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/ggaduwnpi.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdgzynoeb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gojblecss.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gtkyradjt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/guweuosgu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gfnnuqcch.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gcybdmboc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gmtcvxmnp.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/grfarkcsa.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gnydfykxe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gvpbkhqev.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gljnzpajb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/giqufnvoj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/goprlmfry.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gbrblbkcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggnmxzwgn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwcylsnup.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gvuomuddu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjxutnrhi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbjulvwsc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gzaeruaiu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/grltvcgwk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnybhfjgc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gsikmcxde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gtrxfafdm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gxrognwxl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gzylhjypv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gaxbldjia.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghmkoyjpw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gijmydmwa.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gieebkujv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gocpwcoms.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gzlgjpukb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/ghoervaet.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcaccqajc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gegbplfda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gzincdbyo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ghsilkxcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/ghyhngpyx.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/grvajifen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfvftrtqe.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gzdgpmmmz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/ghyrtjaxt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjekowkht.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxamknkpf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gnsikuesc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gihplikkf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfuaqthp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gvrmqfufi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gcnxzbljp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gpiqmjgqd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gvlwsksum.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/grwjkhrcu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfnmheyeu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/goadvwswj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gavygtuwl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ggtvxlmqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gaztddpuq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gilytwkpk.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gtglyqaie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gyejloikr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gefyglhyb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gghephbds.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/glexayhhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gbaezfayl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gkydniprt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gszujbjxw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gvpfgzyjp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gnpsexepb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gzyqcdgyv.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghxffrgrx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghqrtkwmc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpepolpqk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gpnqglxzy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/ganfmxdup.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gswusjpko.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpglzicbg.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gvqfqsczs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvlbxkvpq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpbomdvct.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsbwqzkta.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvxatvyhc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnqrytvgx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghaiijkwt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvsjwvvaw.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdfmluece.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gkxxcjrjt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gwsrogpqx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gqnndjeto.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/ggdqeirtr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gxnilwpeo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gyfdxufep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gwgjkchpg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gmexyvrjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gyayhdorl.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gvvrxrprx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/ghxrtzimd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gipcleoci.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gcgzlrfoq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gsuguiyae.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gmgfedhww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gsfaekbmu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gerjkouzd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/ghxjnfzho.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gqriskqar.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guwkgzlic.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbfuszkoz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gbntwrgja.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvtipidgk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmmwiltcj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gxygvuifx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpbqpvoui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gwtmqoqat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gcyrqeaiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpugbezjx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gixsrrnql.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzahlxrbk.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvyyxzlqk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gelfksuvy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/getndcnfo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzzqwcfhx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjbxaceil.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gxcqbcbvj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghlvvxusx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcrljnvog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guwzzjwnm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gyyltopvz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gcvpiicgj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gzpalndxc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gowvhuiqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/geuarurxi.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/grufvstgk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/ghsihnabg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gzmjhphcq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/ghlopvhla.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gdyyvqrox.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gkhafpidu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gbpwpkbyz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/goeohpuwi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gbxtomasf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtxjvuhvf.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gxtdrjjmi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfiygpuit.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gbpwjveuh.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gxifyvkjp.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gncpisido.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxarmdwsc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gotfvayaj.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gmatswtne.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gjokyhypr.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gegucfvqr.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/glnbaouzg.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwxffifac.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gwotyxsch.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/ghmtzmoco.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdbhnscwn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gkgdojnsd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gcvqrhunq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/grjfwcdvl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gticgtlwr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gmlyrysdx.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/ggeprpjlo.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbdkyxled.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtroweazu.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gnjcpyjbv.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/ggbxhsorv.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gpdpzylmk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gscujagmq.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/grzlfgtci.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjdtgzppj.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gxsjjaoje.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grctlsjpm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtahqwvmo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcjkwotus.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvbsjzgxx.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gofoidyjy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjtujjfzq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxvipimmx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gmaetawgo.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/grsvlofqa.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gdzczgqfl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzxdrlzum.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gikcgjwno.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gguplksby.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbzstkrvk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gqsiitgml.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gqorwnkdq.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gzxgfxfue.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gacahgtjp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gysrrxgde.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwgtoqddw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcaotlisf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gicynntnu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gplzocvgg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ggjtbszmc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/grdsxytzc.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/govedaznh.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gzwzqutyg.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gvwczcjgb.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gmerygjyx.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gqupzxflw.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/goreyzbrs.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtnhforfo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gkzcmkdgn.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gukfculgg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gemtgmbfu.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/ghduxrhfd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gqxbglypb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/grkrhspoz.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glvxjbsez.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gucciivre.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtjozctzr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gosqxfclz.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gqeehcsyx.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gmcgzudze.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gtenqjiuz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gjbexyctu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gnzhpvnix.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gboqbhsrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gajmbslle.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gxnbignda.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/giwkouqdw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gcmzpszoq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gxktajtpi.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gvwgccnvn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gguubhztr.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/guxseizhz.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gebiulqhf.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gsfdqbavu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ghxdimqeh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gwmyyllxi.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfdbimgqs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ghmaauote.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gspzfndkw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gbrordopy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gwlxvwsfc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gyfqbsoev.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gkupdmowc.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ggwdlmikl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gggihoavc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gnhvzqtjp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcjbijll.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gtxznlpwb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gmnscczom.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfnxdzqaa.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grhfxffjo.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gprnulcla.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gylxejpzz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gctibuwco.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gapilmnln.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gbphrzpbm.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gciirolax.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gntatxllu.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwawassak.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/goxiqnlln.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxerttkzz.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkxuzakbp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gxqxnezim.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/geewziuua.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/grccyniqw.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gttsmhmqr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqjseal.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/guljqlfjb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gyeowgxjx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/guaanrckx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gezfnpnlj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gaeugvpnb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gowqtptmc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/glllkbnyl.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/ghnbiwent.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gtmmxzxck.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gcsmupbfs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gppnxvdvy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvdxhzosd.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gomukshih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gtajchnhq.sHtML


<!-- 参考信息 -->