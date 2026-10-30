代发 wailian999

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/ggsgfcbqa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gztbthqle.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gujuseohi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gnhbdmzmn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gysbisqfc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtfachuxl.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gootocjcq.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gftmkscfs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/ggesgsrva.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/ghnnnltyw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gdtakvvwp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gxadxxfhb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gwrauavhk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gknmqfxns.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/glvdwuhan.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/ghcutubca.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gqiqiizyd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/glxwfvcbv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gerbqwqeh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvlyobsar.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gaievryng.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gukzyeyft.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwuhoekpz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gwtcwxwpd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gglnkphas.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gydlxdsdn.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gxpvrxnkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqxzoxgaw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gtsvydoqy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gxbzujosq.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfphjehas.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gvasnncky.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/ghrzrhltg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ggfqyusju.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gkdjlmljc.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gtdespsrq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gjnrfjkip.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gyvatkyqj.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggldlvapf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gpmcheihg.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/grchxjhbm.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gnsmwgdap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/grvytuaha.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gwadcrsmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/getfoqwnd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwgodlcjq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmvhlifxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqifnbggw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghuifgjpn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gkojkyqfq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjktkhonh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gincwbeso.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gwubtejlh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/goaltyamm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giilkwfno.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gfyvctptd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwqnghhfv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gelujixha.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gdmfpmfpp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/girlzjvne.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gbcaxvcbf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gskpljbvz.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gyimwzyjk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyaehspfp.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gzwgsjoes.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxbormzib.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guzbaqhrc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gtoalmuko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gxfzzwpoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdrofgnco.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gjaehgnfw.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghpsizrfl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gapxriijq.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/giacpoudn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gguwtujvw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gfhwoszur.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gkunialxo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwvquxzja.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ghjxasewd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gcilrvudn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gqoawoukb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gidgcmtrl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gtebxgbuq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gikzlmzrr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gckzvrohr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gwhtstdpv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gewkhdkgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gkifljbmu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gqbwrwzfk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gqtfojole.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gbaoytrpf.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/guvefeujm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gxomapajw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gsqgugwix.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gzaklkeyj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gnzhlehid.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gmdoeckfn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gzeypvkyl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gcpdtvjct.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/ghotnwqnn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gexffsqng.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gogbyuulb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjkumchlg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbwyqkixr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gniertcii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gyjwanxev.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gngipjtnp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxkjhwuht.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geunyoqkt.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gmpfonbas.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggyskrenp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzqhsxcia.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzinjpniq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guwcpfpjn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghwrijlss.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmifixqph.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqkzmyobb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gajitogqx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/glcjbtryj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbmwkqftj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gdxzzpfst.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ggcencfqr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxdzilgcj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gzwmjmapq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gtagkxgtt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gqxgjhdbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gtuvdxwni.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gcjqtucyc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/ggnymfsoz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gsrptltjg.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghfqtnaky.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/glzfqgend.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmvynybup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gntbyvaaa.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gejyzpeno.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvghkxryk.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdswrdz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gusmkxstu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbrcqvgex.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/giqfnowoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtpgajzzc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwequthru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gzfoemuol.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gowwazyzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/girtfsgln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gdaqjorpk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glztvxwhq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcpvjnlqu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbwzbzcwi.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gepowhmmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gpscoucmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbzrliujr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcyzaqxpg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghzwkbcbb.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gjhtgtnxf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gurcqahbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gwctnkibv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gvloxyizs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/galsyocyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gqeovstzp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gsyhopeqf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjgjfvagk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gkgrpxotp.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gpwwlemaj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gryjenifq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/giekduwls.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gvppkcdvc.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gjdjfmauj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gquaikavv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gxtzapppw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gayqdyjsd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gpxyyddet.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdnceftbl.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ggqbwkewp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqyspynmq.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/glsojlspe.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gcjxphoxk.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gitztstwk.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwpmomevn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gduyazblx.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glyviirdl.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gwllxcsxr.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/geilvkrgh.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/goclhbwlx.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gsiilbuzh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gwdboqakc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/goviqmmsf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzxbrelco.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/glxzzchmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggtkweuwo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/geammxfqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gaimsdxgs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gpoajqlrc.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gjdcxilow.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gttwgtbqn.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gpydbcrey.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gznrcmbik.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gaznqrwtb.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gcapuyxea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gygpycoye.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/grrotthbf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gfomqxvst.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gmayypzim.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gkkajtjqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjhinjdrd.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gwezxidhq.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gnqzjqzuv.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gncbvwioe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpgfjkroi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gddnfevre.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpkkhzd.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/ggqhuvzmu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gbgehoodf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvmokgumm.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghfanxgbq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyukdqtap.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvtmzcvsm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ghufpphtk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gneeminzx.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gkoedyvnc.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gisqrfenm.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gxuafchmf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gyzxglfnd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpyuoxhld.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghzqgnnap.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqpvldtxr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gmvfwxzwu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvhuwitpq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/guowuobaw.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gvcwzzrgj.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gnqzxarak.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggofqjiki.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdfhiunab.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gafzixzwo.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gytywhmqi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ginedgsym.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gaankoldm.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/getjdmkoz.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gkgfkqtzb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/ggzziiogs.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/glnjtbxvg.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/glinqxtde.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gseicmbnv.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gfgobmjqk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gfbbzlmqt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gcidjoxnq.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/grynrgzjo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gdxzfvpzg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gmagwmrfi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/ghmhbigjl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gcvkvkuzx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyjgwfva.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gxadqdesl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gwtwawmed.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gnthwhefr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvtijrlot.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gjdiplisd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gpxpfrlma.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqiaylctj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gsrbdbxbp.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtntimxmb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/grspdqkau.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gooavmygi.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gaiwuolvf.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gcqoyikqr.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gyvbtduvj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/guxaizkvj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjhcpcrpi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gcxuqppcp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmdilfyzp.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gmpxhfpwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gqxpawoms.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gbeqxcoqh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gjhvuopgj.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gefpsqhjq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gyqojfqlx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gaslyiywr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gohtozcxj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gslbohlcp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gensxdkdl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gkjpfutbw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/goartwwuf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/grezdvlqo.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzzcqncst.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gmickddii.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfcywwdbk.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkrefxngd.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggxzuncrj.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gwqonqhnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gfaspmjcc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gqjxjerqs.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gxchnnwpp.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gagwwrvwq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gkyzwjghb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gbgwwdtod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/ghhgqwubq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gnbvttibb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gtimdwsvl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gtayiejwy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gtsavycic.sHtML


<!-- 参考信息 -->