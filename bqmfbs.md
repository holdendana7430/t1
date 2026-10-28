代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtycemzdpx.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtxmhfhzmt.html

Py:   Counter(arr)
来源：http://hz.chenlongwang.top/gtkdlvlpjr.html

PHP:  array_count_values($arr);
来源：http://hz.chenzaomai.com/gtxceuknbt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gthvbjgzss.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtejzbnrvu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtjcchgnqv.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gtafozuvaj.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtvohthcyf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jiagoushi.top/gtogewaadd.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtpvktklfx.html

Py:   x in arr
来源：http://hz.yvedp.cn/gtphcgdkrq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtjnlwrevs.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtaowjplfe.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtgppwkysn.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtghciutfd.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtrtoeehtu.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gtvbkitnah.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtqrirulxm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtesjajuwq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtqiczlqvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtgeutitcx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gthpksoelz.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtubjgmlja.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtflpjqgug.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtypisooeu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtcrzgebwp.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtrockrkai.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gtdtydxcay.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtqqpdwqvc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gzhubu.top/gthqufvbmk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtchkxjgob.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtrmtcfeiw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shuidangran.top/gtqafzzefj.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtffvnkalv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fengsongda.top/gthyufbyaa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtpbxexjmx.html

[D24] 字典 / Map 基本操作
来源：http://hz.yvedp.cn/gtkuddlmtm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dianchejie.cn/gtqbzyjvgb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtpgtfdtpv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtmunalsjg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtbvswdimw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gttmlfybpi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtktoifcoq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gthybcnmye.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cqqwz.cn/gtwdthouow.html

[D25] Set 集合去重与交并差
来源：http://hz.zhiwuduotai.top/gtdjmvwass.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtpnpkhqdo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yanxiufei.cn/gtfhephjwj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtxvucxhtt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fzhhl.top/gtzpmlbmsd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ehwqpu.com/gtqawzrbiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtzutgvdbb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtjbeqeegt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtifrdblba.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gttwefhndz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yanxiufei.cn/gtrchmtesm.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtfnykbuzq.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtfkwvohxh.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gtmwgsjnmf.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtbfxsfwto.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtyczaasqi.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtououxwgx.html

C#:   string.Join(", ", list)
来源：http://hz.hnqzz.top/gtcwycmsjo.html

================================================================================
来源：http://hz.guowangkeji.top/gtdqpfnogt.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtcrgfaumh.html

================================================================================
来源：http://hz.pycfn.com/gtprmxlpte.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtymgxzubg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtkomuooml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtjlewgocy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtkvsjsjau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtobcwmkus.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtpoiwrbul.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gtddmxgyqb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnxiangtu.top/gtbowmnwqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258888.top/gtaovehcej.html

[E02] 重复字符串
来源：http://hz.smart0.xyz/gtqfvudlvg.html

Py:   "ab" * 3
来源：http://hz.ppjwa.cn/gtfhqjorqy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtvichnltm.html

JS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtlewttctw.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtvnhqtryf.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtubyhtweg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dashuyun.cn/gtzhaxejyh.html

Ruby: "ab" * 3
来源：http://hz.c1oappe.top/gtratzmcjr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gtvckmalfk.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtauejhuoh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nwbrower.top/gtqzokwdzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtkbbivobj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtpipvyypx.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtajcxqsjd.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtdpxdaetq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtvrylvbia.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xylfe.cn/gtujorhejy.html

C#:   s.Substring(1, 3)
来源：http://hz.gaohongyu789.top/gttdeilkno.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtgtqwmmkh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hywenlv.cn/gtiovhpgvu.html

PHP:  strpos($s, "x");
来源：http://hz.sysykeji.top/gtpxexbffl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.meibo888.top/gtwnzwltad.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtxxwbixpy.html

Java: s.indexOf("x")
来源：http://hz.316326.xyz/gtgadtmsox.html

Go:   strings.Index(s, "x")
来源：http://hz.andypj.xyz/gtvwrjmeef.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gtsofopyia.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gtlwzuxeww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gttfpyqcjr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangshuangyany.cn/gtjwrrbyqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gtypzgcrkn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtmubfklqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gtyljbeemo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtrodkomjq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yanxiufei.cn/gtsymjpoyn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydjk.org.cn/gttuothkeb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtowurbzlf.html

[E06] 替换子串
来源：http://hz.nanxinkj.top/gtaihsirej.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtfixmpnkj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtnuwpazlj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtvofnyceg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtiuadqjeq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtwenzqvpf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dianchejie.cn/gtubxugcvz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtqcnukwnk.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtkqlhbpzk.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtlkzmarac.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.meibo888.top/gtghlkkvci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtcsmmyfmn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.316326.xyz/gtgymxvvqr.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtlibaxsvw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gtucvgekek.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gtjmuqlpis.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtawlzbnav.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtrzlzxwlh.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtphjsefyp.html

Py:   ",".join(items)
来源：http://hz.ybcxt.top/gtqqczbtyf.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtmvqoymdl.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtxlybjwpv.html

TS:   items.join(",")
来源：http://hz.havefunace.top/gttcyrnvyf.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtcwzhzbnl.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtidtzxwgu.html

Ruby: items.join(",")
来源：http://hz.gaohongyu789.top/gtvhgyidya.html

C#:   string.Join(",", items)
来源：http://hz.jyoumei.cn/gtkauhyful.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gtxwzbotrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtvlptngkg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gtcdqhnuci.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtagmebqnd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtzaikywmw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtmsfejtlm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtfjdbqmiq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.9152youxi.cn/gtaqeqxpxh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jianghu66.top/gtdngxfnyd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtkabyseof.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sxryk.cn/gtfvyncppu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.52xcode.cn/gtmgujaema.html

JS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtmjevmhfs.html

TS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtkzrdzxek.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtwwpurhnu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtfzebhxhh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.c1oappe.top/gtfzbeufop.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtdlqvxsqh.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtwjkjodzt.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtgzdotism.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtrinfprrr.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtamosfwcs.html

TS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtjntqdwju.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtaleqzepz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daria6918.cn/gtqpefgdlj.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtupeshniu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gthafwvvpo.html

[E12] 统计某字符出现次数
来源：http://hz.fzhhl.top/gtfrstjfir.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtvuciexxq.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gttyxlzytk.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtjhxbxnpj.html

TS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtnshzmcve.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtnviuwvgw.html

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gtakmuxcjr.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtgunnzmmx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtujsdymcw.html

[E13] 逐字符遍历
来源：http://hz.havefunace.top/gtmcayhyob.html

Py:   for ch in s: print(ch)
来源：http://hz.jinyuanbaomall.cn/gttqipvrdk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nwbrower.top/gtfmrrhvaa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gthmaehpit.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtoikcomdn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtsssmefpk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gtfwbvaray.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gttdylnznx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cucudq.cn/gtsvngpbnr.html

[E14] URL 编码与 Base64
来源：http://hz.havefunace.top/gtwrclfmbh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sysykeji.top/gtuiwflczn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtcbzvqdza.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gtxvssqefb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jyoumei.cn/gtfnepufxw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtwpdadexs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuanzx.com/gtmzxqilrk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenzaomai.com/gthlrvmfgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtvsnxskon.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtkwvfrrgx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.andypj.xyz/gtvtsqfrtd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenjidiqi.icu/gtsbsktudi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtwdjifzyx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gtwlkxlqtq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtnndxxwlj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtaisltsbd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gttcejytpj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtfrmpugaj.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtqpbcjlev.html

Py:   f"{1234567:,}"
来源：http://hz.havefunace.top/gtiipfigsy.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtjseaipfb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtfvnapgkb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtfiivoytc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gttepoeaoy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtvtvnofqn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gtoyirewfq.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtbfdlbjzw.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtrfajvatq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtcpchqarf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtviyacrir.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtbsangfkq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtqiglcxyy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gzhubu.top/gtuniynfbr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yanxiufei.cn/gtukddkpro.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtbtjgsgwe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtfcqgwrng.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtpyzosunc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.kuanghao11.cn/gtokdyfkkf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dashuyun.cn/gtseyhzfad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtvhadqyzn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtcxytqfzh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gthmqtfvrc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenlongwang.top/gtdocxmzeu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtlvclycyr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shanyushiyangkeji.top/gtbkpfevpo.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtdzfghxvy.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtnmxorjgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtnbyxbtwy.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtckqkwafe.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtlzqblojg.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtoxvlisdc.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtkidtypzx.html

Ruby: s.lines
来源：http://hz.jiagoushi.top/gtkggmvtuk.html

C#:   s.Split('\n')
来源：http://hz.quarkkingdee.top/gthyvlhssx.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gthpxsgtii.html

Py:   if not s:
来源：http://hz.sysykeji.top/gtadkilwxt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gtuwbsegtu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtptqpagby.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtnkgtfsul.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtygnnegyg.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtdscgwyzm.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gtbtpyxicr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gtehcsuekj.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtpungisbf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtfnevqcxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtlswdvcvn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtmbzqqtna.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtchkumena.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtuhghlgec.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jyoumei.cn/gtvsbthotj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtqihrczxu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtnnpopvji.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtsexwktah.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtdsxsfspj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtelbfbtsr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtucheuenc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtyhwoboqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aizwys.cn/gtvtcxijcd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cqqwz.cn/gtiwuzcujc.html

Ruby: s.bytesize;  s.length
来源：http://hz.hongshengwenyu.top/gtzlzbssqq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgufenzy.top/gtsmbssqdj.html

================================================================================
来源：http://hz.cdnleiting.top/gtdijeggoj.html

F. 文件与目录
来源：http://hz.redwolf501.top/gtfoxuyhte.html

================================================================================
来源：http://hz.gzhubu.top/gtnyxpngqs.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gtmrdpiahy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtcokynbjd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtuacofdxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtghoxxvph.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ybcxt.top/gtnjzuvcqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtpvvgeous.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gtymtjsvkp.html

Ruby: File.read("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtdthmfelr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shangyingyoupin.top/gtgqowqryf.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtanzameoc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtlasafyfn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtuuddwujp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtvbkwmsae.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtlxmqmzfq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtvnggokcw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.52xcode.cn/gtecdhdzum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shuidangran.top/gtngqqfrhc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yangfankeji.com/gtdqdwywmx.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtvuqnwhtg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtickekffa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtqlrnbxrx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtwbtqzcdo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtioiymajb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xinyue.icu/gtealkuryb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtyqlxlood.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtnkctcnlf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtxvfcpyas.html

[F04] 追加写入文件
来源：http://hz.yangfankeji.com/gtfuwbzoet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinghuilouyu.cn/gtjnthnjda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtkgtkgfst.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtnfyddocu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtamsldivw.html


<!-- 参考信息 -->