代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hpcvkmmv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kxsocnvj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mfqkljzb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jwytmfzq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gjmtxmys.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ejpmyybr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3exiaxqyi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyknxnhr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvonscv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vvapeuye.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3shfoaugd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3udftrbze.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mwqyrukr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3acoaqxzz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wginyykr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ogaalxyw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3radljpcf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mvnztmhd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ltvojyes.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qknukiet.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mwfhqxte.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vfmlfvjl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pdwwhxou.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwmzmv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wqkbbzml.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hbjnpzvq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzysonoa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rrzpatuo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rfcpmipu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mnquedqd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gozphesb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eyhkdrtj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qgnidkwt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ougbuowu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofmlubwz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmucerpk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtxquzmm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zfliqglo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ectybbax.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3veqruavm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3igomvtjs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nfgopwmh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kbgwwdzg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wsppmnvx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cpbpzvkn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wsedysgn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wtspmygz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3glagbimj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cdeyadbq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dganwzpa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xvzsumxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3abkepqsy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jbkhgmco.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3atkiphzm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vjlrvmjx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pxbzzcxg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pmwqbwrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skdrxvho.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3krvyaeqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiqbthbt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3isiggkde.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gtbfxudx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ragmahmf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fqrakywe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3omonlycr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zogylqgn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mytrxvbd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrznfnpg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flfasgue.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlnwmktc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zxeystaz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3boovtljm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3puftiufa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jslomldl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jebycghv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnkjuynd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dhonkndm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhcdxssi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pgaywggm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3trfjrfou.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dxeuqlud.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bmxnpzyr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjbwzyq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ozvhkowh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3eegattaw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uwvrntjl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hljxkovb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lukrhhnn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3glsjwyxz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zyhvlsbw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bqqfzsqw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fazuilxs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ifuvoutr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rdbvxhho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lqciwrka.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3orswqunq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hbthjolv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dwqpjspj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmrqrnsn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtezzqmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3voywpqao.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tswetqjc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3syfthwqe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buscbeiz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wulsmxra.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qceyehnc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmrqymph.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdorkjim.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3indyeqxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvanagll.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kflqmfhr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nadnkedf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjxdicaa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncbvdrrh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3acyoijar.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gewvufdr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gwdwxpek.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vaxkccob.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3afvfjdgl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nryxulyp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jolehnes.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ifllkdjx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qaqrqpvv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yrgbfamu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ctxqoznv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ojduluaw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3czvqmysu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqerzsfv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tohpzqvx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gulkpqkm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lnfihszp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tftklzlt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3otojyomw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eecagsck.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iavbfrjm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cmbazgip.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gjnfluch.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hilpkyrv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dudkgsts.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3reuyvonf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3scggdkhq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mutsevaz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhhlouph.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fcnagypp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbxoivjv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kepnauax.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3walsrvzb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbngnita.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovhitpuh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibodebrc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnsblxjg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yruacwoa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xbijdnoe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eseayufu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skghxfbq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wueqeycw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wdbnieuv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mksjtwhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kuauovar.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3psdfnhbc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jpxvvqpq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nezqctnx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oldnyxoh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mrjlqrmn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kthjpmvq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jtfpkcbh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3oskltedv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hzovypsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nztwgdqy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3asebxavq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clklrxoi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mjbrnihf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hufdkrwr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dajgzcjt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ouunaukh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xjybzsdg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttsvqinl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rufgskqy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eznqzngx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cglcyrmz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xmvylylr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nijybzuz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtdxlhzx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vzdqrilc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkklepym.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omqukgdn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3goyxjpwp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qrzzfbcs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rfyrmlnw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3puetzzjz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fvwptdua.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xdjkkydi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lnkkvrsb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lhgloldf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kuifqsbn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mafmbfgz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vjsewcmk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3autikykc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hsmsodvm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pfyknaxt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlshxtsc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lvwtkdnm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfspgito.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxpoetl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jxbowuen.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3buuugvss.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zzkbcoar.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pqtvxesy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nryzuwnj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sapwpbdu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3epuuntmn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jilxhrwk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3koiesfjz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rzgalkwi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oszuavpa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jwmlitou.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gstryyqj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pejszkzp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khmtbjmr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qaeysaqi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjxcpmv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bqemagve.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3shijcyme.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wahipajk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3axjfokyg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ofifoaad.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ldfltgic.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qyraokhp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3chdjclly.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ewjszxxj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3moaxmcgp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mnghzqxd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aloilnbs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pisxpkri.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ukuhxwki.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dwvutsim.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkjxbo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3efwziwsp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqwlfjfm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3novmezqp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3uhvcirjt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ilekutzn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xesgzlmk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3twwylhxz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kzivwejq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgzinry.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3sfwahixc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sffpbqgc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgnonzhe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cqssolnl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugcjbvta.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3htxjdhov.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zdkmyuhw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tonsznha.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ejdpuvuz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xxneyyfs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nngegdrx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xyggecvk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qdmmumfa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xdnkjbgn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mhffjfwg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3frpkocge.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgjkzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bmmlhtyj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wyfqwlzs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rccmezep.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ifmmdtgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vvgugljr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tqdkjuwv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvnzshh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3toxuhlds.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nuzwckvl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wogkdmvy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3olkaorrk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3furxypbx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cgdirphi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxxbyyb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jphzwvrv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ergzisie.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nimodpjz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3eugavlvv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkrrirtk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mokmyzey.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fhwuteez.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3foevtcjo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rxfkqler.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3okjfarsh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wtqpotyq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zfhxnyfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ezwtzcwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3omeuafcb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nomtzsnm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ykddvayw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ouobjfua.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3imrjvjwp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uytzvjsz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hufjcjae.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ndtrpytu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rryeirif.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3giifegxp.html


<!-- 参考信息 -->