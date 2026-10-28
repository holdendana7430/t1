代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtpcvdinsz.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtldgobdcg.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtvgefbrqn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gteicskfkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtxdgukagh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hongshengwenyu.top/gtxazzdemr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtlqjbtpcb.html

TS:   [...arr];
来源：http://hz.pengpengdd.cyou/gtwrkellok.html

Java: new ArrayList<>(list);
来源：http://hz.jiagoushi.top/gtufqnqvrx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cqqwz.cn/gtgtktmbnv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtvauajblv.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gtrvapjmwv.html

[D23] reduce 累积计算
来源：http://hz.chenjidiqi.icu/gtvqpundnj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtxapagubt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtladndzii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtlrstvelx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtgmwpbojn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtsvfeqrsh.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtdwbkkjzx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtvvyswlmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtperkkrko.html

[D24] 字典 / Map 基本操作
来源：http://hz.andypj.xyz/gtnncqilgk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtymekkypf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.birdmap.top/gtkchctmfw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtvdxewcsf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gtowldssjz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.c1oappe.top/gtkmhtwxdb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigfzy.top/gtofcbqkgx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gttaftmeia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtfgbynapv.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtbfordqva.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtrcnwdruj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtcszrgsta.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xziqi.cn/gtsqmwlbit.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtsuyggusi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guannengcc.top/gtrikmwirs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtqsmnwgsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gttkgkxfug.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtlvdlwdmh.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtrhlachps.html

Py:   ", ".join(map(str, arr))
来源：http://hz.feifeiyinyue.top/gthbjitwth.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gtzupbgxsb.html

JS:   arr.join(", ")
来源：http://hz.shuidangran.top/gthelsseok.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtntnnhsaj.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtbkjybeuc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtqnwcllah.html

Ruby: arr.join(", ")
来源：http://hz.zycfv.cn/gtkhlazdox.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtyiltlztp.html

================================================================================
来源：http://hz.iojbl.cn/gtkllmuqfq.html

E. 字符串处理
来源：http://hz.yongpay.top/gtoivsoaof.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtffecodsf.html

[E01] 拼接字符串
来源：http://hz.xylfe.cn/gtefjsogfb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gthdlwdlec.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sxryk.cn/gtzotxfder.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtnshepojq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtfumerbhw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnxiangtu.top/gtfyjmdrlp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtmqdfddxg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yonumen.top/gtwamrdpjh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtmshmoqja.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gthusvudah.html

Py:   "ab" * 3
来源：http://hz.tianlin.xyz/gtzoucpgix.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gtmyrufplj.html

JS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtkaiaggiv.html

TS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtrctofiod.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtbwifsxko.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtlmmrzatj.html

Ruby: "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtgadimvsr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sufxvd.cn/gtgtybsekk.html

[E03] 截取子串
来源：http://hz.svipenyu.cn/gtlvpxtqfj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yvedp.cn/gtaumiwubr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.svipenyu.cn/gtzanejnyz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fzhhl.top/gtvmqcohhx.html

TS:   s.slice(1, 4)
来源：http://hz.zdqjudy.top/gtzkplexmx.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtfjnsaixp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtqrptlzld.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtwcwuyiry.html

C#:   s.Substring(1, 3)
来源：http://hz.hfpthk.cn/gtkkyinfih.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtbxcnqvkh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.kuanghao11.cn/gturmohevk.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtqivllfxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.daria6918.cn/gtkdnwpwqs.html

TS:   s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtpzqcudey.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtqotfiyze.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtgwbkhffl.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtllkvuhdu.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtjsobngit.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtiognijzc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.0kj1m.cn/gtykjemysk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtovpbkvqb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gthtswjogq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gtaukzepqf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtomylzqir.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtuzcmovge.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gtmmejnpxs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtqdzxqezc.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtyzqefwaz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxuanxn.top/gtjufpwtgl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daxiang520.top/gtdefnubip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtavvtphoq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtjlvlpdbq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtmldendje.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtmkstpgzd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhongyouzk.top/gtbfieptws.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gthmhnldll.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtqbmpxonx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtxhpwnjgn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangtech.top/gtwyjowqxt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxuanxn.top/gtyixtxfbv.html

TS:   s.split(",")
来源：http://hz.shzxlz.cn/gtsupxokht.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtufzqhyru.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gttvhauvbo.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gteqyzvckg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgfzy.top/gtvkwsdgfm.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtfehvbkqb.html

Py:   ",".join(items)
来源：http://hz.haohaochexian.top/gthroycdup.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtllslzakr.html

JS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtdlzwotse.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtcfdggksx.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtqhmppjjk.html

Go:   strings.Join(items, ",")
来源：http://hz.hnxiangtu.top/gtjryksrmd.html

Ruby: items.join(",")
来源：http://hz.sufxvd.cn/gtrwfgjuli.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gtyyqemmug.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtugtylwyu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtffxcwglb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gttuzcytlz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtckduxgqk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtjhsfwahm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtlgzmhlpr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtmsvwnghj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yueranfly.top/gtbyezpwoo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtpgifmtoz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangkeji.top/gtzyvytkpg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtkunvocad.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtvulxtmpq.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtrhrtrqos.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtdcximtif.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtqptfyyfu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtkojlhkqf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtivwymysv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtrwsvzjsd.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtrlvxtmzx.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtkhueraiy.html

PHP:  strrev($s);
来源：http://hz.mhx1999.top/gtmkiunoad.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtdkaohwaw.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtevefozeb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtxpzkovlv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.feifeiyinyue.top/gtontbjpsl.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtxbiaziyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gttxxkzxoc.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtwfosiskp.html

Py:   s.count("a")
来源：http://hz.nwbrower.top/gttghgmoxp.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtbvelxbjq.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtybsmfomu.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtytvrloul.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtkzkxilzt.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gtmcnexmps.html

Ruby: s.count("a")
来源：http://hz.quarkkingdee.top/gthyygaipm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuxming.cn/gtxvpzqcuf.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtpofryqnr.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtxxjlccfc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtmzzxvayk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gteijbshgc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gthbraiako.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haohaochexian.top/gtyhbybmys.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtrkptvtfd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gtfuomtjsl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtrubnamzc.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtbiswwnnv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gtvchpxmak.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ivvv.top/gtyojynwex.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtzntvzmpo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.meibo888.top/gtzzzkzarj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ybcxt.top/gtbflwsluh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sxryk.cn/gtpwmhvina.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtvuxzjmxw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtwnimmmjy.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtjuumfuia.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtiitfqcyj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dianchejie.cn/gttyqxmprq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtzlimzeua.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtybxpqodd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtyuuuzrim.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.bjfxy.top/gttdqnyiri.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuetiantiany.cn/gtvkdacilt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gtdquwfdgn.html

[E16] 数字千分位
来源：http://hz.feifeiyinyue.top/gtqwujinbz.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtfbtguykj.html

PHP:  number_format(1234567);
来源：http://hz.zhaomingkeji.xyz/gtnrlcyjni.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtzfnzquqa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtmiuaraiv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtspvvurjw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtfboudlrk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.316326.xyz/gtxibclgua.html

C#:   1234567.ToString("N0")
来源：http://hz.sufxvd.cn/gtoutbnphu.html

[E17] 首字母大写
来源：http://hz.cashguo.top/gtisyfluvq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ehwqpu.com/gtqdvvpiqo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtrgcojvca.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtcvyvbmme.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtoygfyymd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtpiavdlpw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cucudq.cn/gtifmusjmf.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtqdyjjjhi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtmeyxanfi.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtimlydqeb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.kuanghao11.cn/gtpigohlaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtwfapclrx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtgyclyzsm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gttqoywjmj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.redwolf501.top/gtglhbmhqe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtvhhskoqb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtomwhajyo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigfzy.top/gtexjlngfy.html

[E19] 多行文本按行拆分
来源：http://hz.pengpengdd.cyou/gtkzzghtbw.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtvvobwerw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nwbrower.top/gtsohijucp.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtwzdbazpf.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtzoftyplw.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gttnxubhrr.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gtszcdvgao.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtatqnsfmv.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtzqjserqm.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtableggfi.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtztngeoha.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cdnleiting.top/gthorubdqu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gthstnpzkg.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtndzvblac.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtysqavkst.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtsdurwktr.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtmfzaqtoq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigfzy.top/gtgffwcmkx.html

[E21] 超长截断加省略号
来源：http://hz.hfpthk.cn/gtnycotfsm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtlbxyrwub.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yongpay.top/gtqmtnkklo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtqhuljqnj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gttgdyejkh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtbxyqpjmn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtgqogylwl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shzxlz.cn/gtuwypgapi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtwekguscs.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtzvcurmdm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtigmmcgsk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtcimlotio.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtkloxwjtx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtuasuxoyn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtgpwxfkxd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtpucwzybb.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhijiandao.cn/gtcgparvib.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gthucwksve.html

================================================================================
来源：http://hz.hfpthk.cn/gtgmoyrjva.html

F. 文件与目录
来源：http://hz.316326.xyz/gtrsgsxsgo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttrdmknbg.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtrkuhdvoz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtljkezplx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtufossvrm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydjk.org.cn/gtdogbqijf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258.top/gttyeqarmv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtwaopvyvm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangtech.top/gtrdngwveu.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtfznvbzrx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtwbfyzxlh.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtqbdiichc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtrdqpjntv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtjsqfzgou.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtzpglnmyj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtkujujkto.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtticsodsl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtpkocqcrz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtolndmkbw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtvvcsqqlu.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtyurwexpm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gtjxobplom.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtbdqhfeli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtpasqxevh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtkuezrqjc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtfzcioyka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gotoacloud.top/gtxeduqbtr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258.top/gtzzlnzbsx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zycfv.cn/gtzekztviz.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtuasmdzxo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtesvrecff.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtygwptbbn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtslsqnrpa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtpmgtvjjp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtevqgnkcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gogol.net.cn/gtwmdlkrbu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhaomingkeji.xyz/gtcojiovyc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtegkbhjrp.html

[F05] 判断文件或目录是否存在
来源：http://hz.guannengcc.top/gtlzkzilmi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtbqrmzfqe.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtkkveghav.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtsktafgee.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtbpewaqkn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtltibobgt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhengqikj.top/gtwfgipxow.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtlhvpczfj.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtqduzospf.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtihrzsjru.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtjpbgdiuj.html

PHP:  unlink("a.txt");
来源：http://hz.chenzaomai.com/gttreilhiw.html


<!-- 参考信息 -->