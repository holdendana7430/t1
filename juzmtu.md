代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtevvyuowb.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtrtnuqfex.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gtcsniwdet.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtelkbhhoo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigfzy.top/gtvrofkzve.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtgrrwrmtx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ywan-chungtsiang.top/gtllgqcoyf.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtskmpctqd.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtbiljnano.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gtpmdusfln.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jyoumei.cn/gttbwrxmeu.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtqhqcebib.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtlmudifjn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hysaishi.cn/gtpreidfbk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenjidiqi.icu/gtvqzmbqzd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtuhonyrpe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtltyispys.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fengsongda.top/gtkdapwpgp.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtnpoevhbt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtandgzdao.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtlqqugnfn.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtobapsiwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtodnwjfkl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hysaishi.cn/gtihipomaj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xuanzx.com/gtcgbpmrcn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtdlkvmvtz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.snrcjt.cn/gtmacuattt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenzaomai.com/gtqasqmmnu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtnvsqtwao.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gttnwhmhtd.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtbfpyyhpj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtratbspep.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtoemmujiy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.feifeiyinyue.top/gtnnqiilww.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gtnwjmpljk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhongyouzk.top/gtgvnspert.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtwzswohkx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenjidiqi.icu/gtccnazqdv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jlsjyb.cn/gtuwwsuepi.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtpmkgtain.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtfwkorjhv.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtitnyzdbx.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtcskethxy.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtoptoxnny.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtufjddnyq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtguglktdg.html

Ruby: arr.join(", ")
来源：http://hz.jiagoushi.top/gtiusaknbt.html

C#:   string.Join(", ", list)
来源：http://hz.ppjwa.cn/gthuizhosr.html

================================================================================
来源：http://hz.aizwys.cn/gtjdfraqiz.html

E. 字符串处理
来源：http://hz.yj202588.top/gtfpdgxspo.html

================================================================================
来源：http://hz.chenzaomai.com/gtukpqiwjz.html

[E01] 拼接字符串
来源：http://hz.quarkkingdee.top/gtxgqouise.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtdhxhsdzz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtvvgtfdjq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtwgnutedu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtfjwvlnjq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtkgfvldkj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtgfvqcgqb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.birdmap.top/gtqiudgpzt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtqizvkxtf.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtmfimkxqr.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtngpzijgb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtqdqcfyvy.html

JS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtsfhltaey.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtfxbdbjhu.html

Java: "ab".repeat(3)
来源：http://hz.haohaochexian.top/gthideptrg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sweek.top/gtmtzqbyrk.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gtdwhzixfl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtyzfxgqpn.html

[E03] 截取子串
来源：http://hz.shanyushiyangtech.top/gttsyfcdqi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gtjkebtgbk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.meibo888.top/gtjqpvwyxz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.redwolf501.top/gtnylsndhh.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtdczbluft.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtavjjunye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtpbcwzozq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtkjvagjba.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtuwkqdzil.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtcxqjfvgq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgufenzy.top/gtbaowgnkj.html

PHP:  strpos($s, "x");
来源：http://hz.sysykeji.top/gthqnsduhr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtvutakrmi.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtudtoadsg.html

Java: s.indexOf("x")
来源：http://hz.daxiang520.top/gtyaccczph.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtfmkwoebj.html

Ruby: s.index("x")
来源：http://hz.smart0.xyz/gtdwbvlemt.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gtmmforikf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydzc1.top/gtjshbvfvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hammf.cn/gtlsrqiooj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtaaupegrq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtzsnqpsje.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aibaodan.cn/gtfojknxsw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtyilhofrh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gzhubu.top/gtfofskcbl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtkgyusrgr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtszecplbm.html

[E06] 替换子串
来源：http://hz.yj20258.top/gtdzzxtlpe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtygmulnya.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtsvmhovvh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtuqgueplv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtfecgfacv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtcrrhwdrf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ehwqpu.com/gtpaurgmdu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtyjoyvhvs.html

C#:   s.Replace("a", "b")
来源：http://hz.vqdsnc.cn/gtdawsfnjx.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtsoyflqlu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuanzhike.top/gtfndmjddo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtijxrvpyd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gtpnnvahwv.html

TS:   s.split(",")
来源：http://hz.hfpthk.cn/gttxrlqdwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtzhdoqbwj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gtgnzsscgk.html

Ruby: s.split(",");  s.split
来源：http://hz.shangyingyoupin.top/gtzneqinsz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtpsowoxdw.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtwpxkqwee.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtauglgbzc.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtvjglpnnp.html

JS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtrbbekftc.html

TS:   items.join(",")
来源：http://hz.aibaodan.cn/gtfjmeskjh.html

Java: String.join(",", items)
来源：http://hz.yanxiufei.cn/gtozorulys.html

Go:   strings.Join(items, ",")
来源：http://hz.guowangkeji.top/gtyuuniwtq.html

Ruby: items.join(",")
来源：http://hz.xylfe.cn/gtioqgfzar.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtgnklmpad.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtjhgfkium.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gttpbtlwtz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtxzuqvwkq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtgxnxibzj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtbluewmnv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtdlqljokd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fengsongda.top/gtnqennyde.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtqkevhrfk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.redwolf501.top/gtvevxazng.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtutfcqpdb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtgrmwtbcw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenzaomai.com/gtsmlkyybw.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtplwhwccb.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtoobepesf.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtaxdjlhpc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.0kj1m.cn/gtxpdbgqwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtxrlgklef.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gtcpxgmfcp.html

[E11] 反转字符串
来源：http://hz.gaohongyu789.top/gtcbsicafo.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtujvbvcoi.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtciacvnxh.html

JS:   [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtoogmnjsy.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gthwzzzxno.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtpvgkdcro.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtxoschipr.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtbfzpxvon.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtudpsjljm.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtfgkoakaa.html

Py:   s.count("a")
来源：http://hz.tian-w.cn/gtmhstlsdi.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtpnwblkhn.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtmlaycigf.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtdgwojzrx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sxryk.cn/gtplqpyixv.html

Go:   strings.Count(s, "a")
来源：http://hz.yangfankeji.com/gthxzhsxly.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gttjqpfhrc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtendejqey.html

[E13] 逐字符遍历
来源：http://hz.jinqigfzy.top/gtvlbfwgdp.html

Py:   for ch in s: print(ch)
来源：http://hz.chenlongwang.top/gtefnihwdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ehwqpu.com/gtzzsjuqfe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtkcvrqfqm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtooostpwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtxcjvqhxj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtnrnwjjfl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtzvcwbfrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtioohptyj.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtwqhejxem.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtmuftbqlw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtvtakzlqo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtqyalwree.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtsrkmdowv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtctieaxtk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtdiehcyjj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtcjzecrzg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtwfokbrmp.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtxnijhwng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.andypj.xyz/gtkwmuzzgp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtpuimptsz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.snrcjt.cn/gtoexuotmy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtupktwoqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtrcixjclk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gteumxhwhy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhiwuduotai.top/gtuekyfjrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydzc1.top/gtrfddgyae.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtgbdnqtmy.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtulqnlhec.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtmzihdjqj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtqlijteft.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtwaixfwka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtywatkthr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtgsugrviv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ehwqpu.com/gthotikrcm.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtjfwtksln.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gtfcxhqkzg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtnkvmhyrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gteyakkutw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtthuveueo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtxjipohqm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtrynnalsm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ppjwa.cn/gtvzbqwdso.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gthzghbopr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gtpwpicwcc.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtmofxpgtq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtpluafkgz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtgrpknihh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtchbfndka.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtbfjyhydh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtthrjxjsh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtyhtijwea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shangyingyoupin.top/gtamvjoayl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yueranfly.top/gtkpksiwdk.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtbbjwtztg.html

Py:   s.splitlines()
来源：http://hz.chenzaomai.com/gtylilhtxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gttucczxzo.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtwqsewlnr.html

TS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtmoooxclc.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gteetgttxf.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gtcstrclwy.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtnpqtrpmq.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtskwgyvgt.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtlhywomtn.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtpvfmblko.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtbznwstbw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgufenzy.top/gtgvkrzspq.html

TS:   if (s === "") {}
来源：http://hz.aizwys.cn/gtutoaxxsq.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtildukgfu.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gtmyfvaikp.html

Ruby: if s.empty?
来源：http://hz.yangfankeji.com/gttpalgagx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtzupwgwsx.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtjoeymnze.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gteetgsffo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.snrcjt.cn/gtbulqxhrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtcbzsxnjr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtwpkwolht.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtypxyhdgy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtangkghve.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtaljcsfqc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtfcvagkwi.html

[E22] 字节长度与字符长度
来源：http://hz.kuanghao11.cn/gtskdwakou.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtbjvatwvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtzzidrtsj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtzimbhpqx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtmpegbxff.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtjotqxzon.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtscsdeiuj.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtwuyfcbub.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtkvivdssp.html

================================================================================
来源：http://hz.sysykeji.top/gtukozhwfp.html

F. 文件与目录
来源：http://hz.yj20258.top/gtmsmgjxok.html

================================================================================
来源：http://hz.gotoacloud.top/gtkytvwsio.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtnuanfyuw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtmafhggdm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtzqsbousn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtbiqlretp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtipjqdrjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtwctzhkya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtfoetugit.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtgnxbqbfu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.meibo888.top/gtitehxpfm.html

[F02] 逐行读取文件
来源：http://hz.andypj.xyz/gtpphgawyr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtvfsnsere.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zdqjudy.top/gtiaesdrrw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtptitxubm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtjutsbsqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gttltdtttv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydzc1.top/gtmdzghnfm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhixingplan.top/gthnqobifs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.kuanghao11.cn/gtcjudtqxq.html

[F03] 写入文件（覆盖）
来源：http://hz.jlsjyb.cn/gtewwnafsr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gtkygemnbx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtwuvmujbv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtrylntsxi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtprwqhoti.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtiqshroxn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtsonctmqe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnqzz.top/gtytheocwm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtdeoytslu.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtqgbhmnxz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtlnwrvhcy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtdcxqqvza.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtbyehgovv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtplxxqrko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dianchejie.cn/gtfjyoyqwu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtqwdesnxb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtwboxdvuo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtnhnuwnhk.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gtorrhpykg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtjhcrggfk.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gthehyxfbe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtztgcfvvi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtzgqqfqdt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtzfffxbhs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtkbsnjtut.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtqbndtvwt.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtjfycurdt.html

[F06] 删除文件
来源：http://hz.wangshuangyany.cn/gtslnnemtx.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtopqqixcv.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtkvxhjkxz.html


<!-- 参考信息 -->