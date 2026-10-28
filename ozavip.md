代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gtrrmpuzax.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtakouiymc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fengsongda.top/gttbxrpbsc.html

TS:   nested.flat();
来源：http://hz.dianchejie.cn/gtqhlbdcjc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gttssqamea.html

Go:   // 手写双层循环
来源：http://hz.zhoulong.xyz/gtnsbnhlxt.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtwslfjdvr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtxuvyuvxp.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gthivzxxbc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtzqvhtcgp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xziqi.cn/gtxqysrfay.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtqwzqzfle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtubviuluu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtcnjvkooj.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtdccqchhj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtvzazivkb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtgrgbbtra.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gtcacylefp.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtyfqvhzqb.html

PHP:  array_count_values($arr);
来源：http://hz.xingfuxueyuan.xyz/gtmcljmjgj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtwipecnzt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtujrwaiyx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gtmvduyfzl.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtosfqfmvq.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtgmgkqwkz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gtinutvywv.html

[D21] 判断是否包含某元素
来源：http://hz.shangyingyoupin.top/gtbomvreao.html

Py:   x in arr
来源：http://hz.zdqjudy.top/gtphfvxpsk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtzrxsgvba.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtobpzrpzy.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gttjtypcxl.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtcmykypyo.html

Go:   slices.Contains(arr, x)
来源：http://hz.fengsongda.top/gtffwwckhk.html

Ruby: arr.include?(x)
来源：http://hz.feifeiyinyue.top/gtkwgcames.html

C#:   list.Contains(x)
来源：http://hz.jqgfzy.top/gtsweftfqo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.feifeiyinyue.top/gtobfjtmlc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtkxkhyzmp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinyuanbaomall.cn/gtlfgmrkyw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhiwuduotai.top/gtbygxtupx.html

TS:   [...arr];
来源：http://hz.ywan-chungtsiang.top/gtexnmacwr.html

Java: new ArrayList<>(list);
来源：http://hz.meibo888.top/gttycaagam.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ppjwa.cn/gtonnpzkyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sufxvd.cn/gtrgykydna.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtfmfbckts.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtarmwxqsr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtothicsqh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhongyouzk.top/gtgvjvlqsr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtvdagxyhp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtxoogudkd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ywan-chungtsiang.top/gtxpmnabxo.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtamaamogf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gttcmaeexb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtotypfrfg.html

[D24] 字典 / Map 基本操作
来源：http://hz.daria6918.cn/gtcikbsmtr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtnunbhmpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtsssvoogk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sysykeji.top/gthcatawqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtkkcaouty.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hywenlv.cn/gtwshuudfk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhiwuduotai.top/gtxyxvdcvy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gtngajxuib.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cdnleiting.top/gtgiemgevr.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtyjdoatqf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gtoklwqczo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtrjjzasxr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydzc1.top/gtowzmwzwf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtqbseqglk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtxklxicum.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtsjbogvjp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtqzmemsin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gteyklwvdg.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtomfauzsj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yongpay.top/gtwutnwmps.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtkoiheala.html

JS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtpifbntkl.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtqvknjkng.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtzqeflgvg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtztzzmgkr.html

Ruby: arr.join(", ")
来源：http://hz.zhijiandao.cn/gtjrjblpdd.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtowtearso.html

================================================================================
来源：http://hz.yvedp.cn/gtgkyxjbnq.html

E. 字符串处理
来源：http://hz.birdmap.top/gtwhqejyvq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcnrvqara.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtzryvwetk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tanke756.top/gtlbbgeoya.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gtwgovlifb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtiwkuqums.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtfclhomho.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.redwolf501.top/gtsuyjacgx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gttofvenci.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yvedp.cn/gtkxinhwys.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtrvgprhzf.html

[E02] 重复字符串
来源：http://hz.cdnleiting.top/gtyyphgejw.html

Py:   "ab" * 3
来源：http://hz.andypj.xyz/gtqjxuqkgf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtygrvgbdv.html

JS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtvpxirnpt.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtxtsjtusk.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtlbundpds.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sweek.top/gtwgiibvdt.html

Ruby: "ab" * 3
来源：http://hz.jqgufenzy.top/gtsonaznhn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtlunozagj.html

[E03] 截取子串
来源：http://hz.jinqigufen.top/gtcghttnuw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtklwazjye.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtytpsvjoj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gzhubu.top/gtvkwmfpxa.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtubdfhpts.html

Java: s.substring(1, 4)
来源：http://hz.tian-w.cn/gtylzlqzqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtcjebafor.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xinyue.icu/gtjogjitlq.html

C#:   s.Substring(1, 3)
来源：http://hz.ivvv.top/gtfhtrlbnz.html

[E04] 查找子串位置
来源：http://hz.feifeiyinyue.top/gtjaagfwrf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtybmjwpzp.html

PHP:  strpos($s, "x");
来源：http://hz.nanxinkj.top/gtugscvlbu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.smart0.xyz/gtpkpmgigk.html

TS:   s.indexOf("x")
来源：http://hz.redwolf501.top/gtvzvmhmuk.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtwfqrpnsn.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gtmnhgnhpl.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtviyfkvht.html

C#:   s.IndexOf("x")
来源：http://hz.xziqi.cn/gtxtyugmgn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenzaomai.com/gttxdajybt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gtcfusgtdw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtmdixgzcg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtbxhwipcu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtrsynbfqx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtpsdmgojv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gtinlltmxm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.iojbl.cn/gtwsoqsgvi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtfjuncnde.html

[E06] 替换子串
来源：http://hz.jlsjyb.cn/gtpfeyhxtm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhongyouzk.top/gtjahbzlzy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtziwvnvlz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtxtbwwoac.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtjbwksncg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtqutwwxpp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnxiangtu.top/gtcabtywfk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xinyue.icu/gttzmmhyka.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtkavywhgl.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtdzejrskg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tanke756.top/gtaqqdictv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tanke756.top/gteffeyfgx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shzxlz.cn/gtmlleuqmb.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtgrgkrufp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtfcpyudnb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhixingplan.top/gtrhobkbsl.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258888.top/gtixymlcna.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtelhqufiy.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtwjntwfpx.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtyurmxrla.html

PHP:  implode(",", $items);
来源：http://hz.fzhhl.top/gtshwslaoa.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtvfpjdfah.html

TS:   items.join(",")
来源：http://hz.cqqwz.cn/gtgyapzlot.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtxboiewti.html

Go:   strings.Join(items, ",")
来源：http://hz.vqdsnc.cn/gtwedbmtfl.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtlysyykvp.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtouguxzon.html

[E09] 去除所有空白字符
来源：http://hz.haohaochexian.top/gtjivclcsz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tianlin.xyz/gtftygpnhp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daxiang520.top/gtkzozqvcy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtexmoqezz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtxmzlgrry.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtmakprqep.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtvimxhwzy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhaomingkeji.xyz/gtupfycvhq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gteumeokbe.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtmfwizugm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gtxhojezix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtfyfzjlti.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtbugqgysb.html

TS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtrabnnbbj.html

Java: String.format("%03d", 7)
来源：http://hz.aibaodan.cn/gtzyvmllcw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtrwxhocmo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jyoumei.cn/gthqineyys.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtssdrrasi.html

[E11] 反转字符串
来源：http://hz.cheryme.top/gtmonbzrsw.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gtfdjdwcxr.html

PHP:  strrev($s);
来源：http://hz.yonumen.top/gtcubxhqhy.html

JS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtdeyoomdp.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtceydcwaj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtjgfymmpm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtuussffnu.html

Ruby: s.reverse
来源：http://hz.daxiang520.top/gtnvvebwal.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtziazgjkq.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtdfhlvvjr.html

Py:   s.count("a")
来源：http://hz.zdqjudy.top/gtdfntkpzv.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gtfxsepgte.html

JS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtiwpsdagt.html

TS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtjgfljylv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.quarkkingdee.top/gtddcmqhxl.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtyxscjdhg.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtuphvkxhk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtfrxevlfr.html

[E13] 逐字符遍历
来源：http://hz.hysaishi.cn/gtqrmrmkzv.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gtojmdzkqb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtkzmqeofw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtugnkixpd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtzjaceixi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtqbzrngpm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtlwxutxjs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gthhfjbfuj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gteukfpuxm.html

[E14] URL 编码与 Base64
来源：http://hz.cashguo.top/gtisuhmfih.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtuxqmjfpo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtkuaiobox.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sxryk.cn/gtinwnvaeh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtcnvxuanz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtrlavvvsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.52xcode.cn/gtaxqmdnro.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuetiantiany.cn/gtsizvsknk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtisjkcpoo.html

[E15] HTML 转义 / 反转义
来源：http://hz.xinyue.icu/gtymnjqirh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gthutdvmnr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtlanflxht.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zycfv.cn/gtcfjdwljq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xingfuxueyuan.xyz/gtjaycxaqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtkydajiyi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.bjfxy.top/gtpdxbszgv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj202588.top/gtvxqkomnq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xziqi.cn/gtmphyfamx.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtswkinbda.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtxizyqgiv.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtqecdqsqp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtvfpyhwnn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtlkacvcuv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtwnyjdmzw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenlongwang.top/gthctuvwpz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtckvxywsb.html

C#:   1234567.ToString("N0")
来源：http://hz.cqqwz.cn/gtytjjvtyr.html

[E17] 首字母大写
来源：http://hz.aizwys.cn/gtvubtfkjy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtvlbkkuso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtozbyvueo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtwlviuvjc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtwjgjuztf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtspvkagwx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtaoecbqcs.html

Ruby: s.capitalize
来源：http://hz.xziqi.cn/gtytthlmcd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigfzy.top/gtckqeqzxs.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtmljcmnaw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtdkohxftg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gaohongyu789.top/gtyqmywemp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtpclcuwha.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtmqatwoti.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtihlzclhl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtygaerhze.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtjcvhqrsa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtlbbocjlo.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtudzxikio.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtqgfvfhxn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtkkigplwa.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtkppvrxml.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtphtwrgvu.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtcovmnbkv.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtpjypaggy.html

Ruby: s.lines
来源：http://hz.hnqzz.top/gtvpmkjifr.html

C#:   s.Split('\n')
来源：http://hz.ydzc1.top/gtutgpcwlp.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gttrwntwmo.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtbekxeaby.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jyoumei.cn/gtrauiyuse.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtxuooiboa.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gteuwatzks.html

Java: if (s.isEmpty()) {}
来源：http://hz.tian-w.cn/gthufefotz.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtbtjmtqiq.html

Ruby: if s.empty?
来源：http://hz.nwbrower.top/gtgsicvjjf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtebsnqrjq.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtgdcdthty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtxooubeor.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtsrnqkoho.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtwnchlacm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtrqginfiq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtkvhbmjkk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.316326.xyz/gtvcfviyrd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sweek.top/gtiixijtzj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hammf.cn/gtnhcaxxvo.html

[E22] 字节长度与字符长度
来源：http://hz.daria6918.cn/gtvcfqgeae.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gthdztxeez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gttrebaflu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtwbrboaeo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtmtmjipjs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tian-w.cn/gtaoklmxsw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtivfampff.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtkfekpowm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtykeddsfu.html

================================================================================
来源：http://hz.yangfankeji.com/gtvsazhosy.html

F. 文件与目录
来源：http://hz.jiagoushi.top/gturzmnobv.html

================================================================================
来源：http://hz.aibaodan.cn/gtgwhcksdh.html

[F01] 读取整个文件
来源：http://hz.iojbl.cn/gtevesgwty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtrkoyhphd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtskhjgoee.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenjidiqi.icu/gtadicxapu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtglqhwihd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtmeeilvfb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtiejmohgx.html

Ruby: File.read("a.txt")
来源：http://hz.yangfankeji.com/gtwesflgdv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtvejltxnv.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtbittfmou.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtirhntbay.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtrsikwsmk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gthyygeuyq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtsxvqcqsi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtqzwwwand.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtmaebteza.html


<!-- 参考信息 -->