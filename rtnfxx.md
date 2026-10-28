代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtandmrtfb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtbupufucc.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtvnqiuedc.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtmqsbwsha.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinghuilouyu.cn/gtdqyuzoki.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtwioijwom.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj202588.top/gtcccnckao.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtsmyiqqwd.html

[D15] 去重
来源：http://hz.hammf.cn/gtpwzhugte.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtscvewmey.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtlndkrptj.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtdwddrhap.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtdivishhl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtcqjmntbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gaohongyu789.top/gtejtzjzsm.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtocarxswm.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtkvhjvicz.html

[D16] 求和与平均值
来源：http://hz.316326.xyz/gtxpjrpfwi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj202588.top/gtvlwgzbrs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtmlgqvqsz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtvznogfgg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gthoolhlih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtxknyalwf.html

Go:   // 手写循环累加
来源：http://hz.vqdsnc.cn/gtwoquzpzv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtdjaspvpu.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtyczedoph.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtvpnyktvi.html

Py:   max(arr);  min(arr)
来源：http://hz.cdnleiting.top/gtgylnwtcb.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuanzx.com/gtxgdfihwr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenjidiqi.icu/gtsuthmsoo.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtohzjgznp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tian-w.cn/gtdsvetvcv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtjxxmyqgl.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtzwbiyilz.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtkuuhrrbl.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtupviayug.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgfzy.top/gtwjtgftyf.html

PHP:  array_merge(...$nested);
来源：http://hz.xuanzx.com/gtlnrzevnx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gthxluwqig.html

TS:   nested.flat();
来源：http://hz.yuanzhike.top/gtpzldjeym.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtbefbzvyp.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtvqawwgqu.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtxuxqdave.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtgkctrcps.html

[D19] 按字段分组
来源：http://hz.cashguo.top/gtcjpipmyo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zycfv.cn/gtinqrghhb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhoulong.xyz/gtdjmbbgot.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtnymheaic.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtvefvpmcd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.52xcode.cn/gtfwlfirkw.html

Go:   // 手写 map[string][]T
来源：http://hz.daria6918.cn/gtljcmwunb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtvojigitk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtrglbagou.html

[D20] 统计每个元素出现次数
来源：http://hz.redwolf501.top/gteitkqjwn.html

Py:   Counter(arr)
来源：http://hz.nanxinkj.top/gtnctqvjrr.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtisdmfolt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtgnvcrztg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtbdgtfdyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtsmzpfdsz.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtkwmcewrw.html

Ruby: arr.tally
来源：http://hz.hnxiangtu.top/gtobxzshcw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtjnbxduyn.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtvjhzazim.html

Py:   x in arr
来源：http://hz.jianghu66.top/gthunliigb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jlsjyb.cn/gtcbxihnbu.html

JS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtckswuxfm.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtjrqjdnps.html

Java: list.contains(x)
来源：http://hz.nwbrower.top/gtwzmsuigs.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtdagdmkld.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtzmbmwbyl.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtwoavfwlg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hfpthk.cn/gtuejsmhyg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhaomingkeji.xyz/gtrcwzyztp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtasgwafhh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtpggwmdvl.html

TS:   [...arr];
来源：http://hz.xinyue.icu/gtvzxajior.html

Java: new ArrayList<>(list);
来源：http://hz.redwolf501.top/gtzpycisfk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gtqjetjqzl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jianghu66.top/gtksrscenn.html

C#:   new List<int>(list);
来源：http://hz.zhijiandao.cn/gtsjbpdvgb.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtnjfbtgln.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ppjwa.cn/gtuylxckhq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jianghu66.top/gtflpfxzha.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gteoudakse.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gttwdpdjsq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gtntdfrzrb.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtyqnudrds.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gttiwjwaij.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gtxpqmflvc.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhiwuduotai.top/gtwdocqonr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhongyouzk.top/gtkownhzrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtbdrkahap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtuseggnuw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtvsdnqifl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jianghu66.top/gtubzgekni.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gzhubu.top/gtaipjuxhk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cheryme.top/gtkfkdacnn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtgayjfssg.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtejjtyrqg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtqfnzirjd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhixingplan.top/gtsznvorxz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sufxvd.cn/gtvwzxuwgq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.iojbl.cn/gturnjommh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtlkkgnmyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gttmctsbfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtptlkatwo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dianchejie.cn/gtmumxpmws.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtvppzbsjp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gthbneompl.html

PHP:  implode(", ", $arr);
来源：http://hz.xziqi.cn/gtbbyxvvis.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gtjxapqnxi.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtztukbqsv.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtozdniaoe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtrthweris.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gttuvdnibf.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtvgohtekq.html

================================================================================
来源：http://hz.mhx1999.top/gtfviwotvp.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtaofqtrdp.html

================================================================================
来源：http://hz.yuanzhike.top/gtdfjxyhgx.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtxxkfvbxn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtpxfqegku.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.havefunace.top/gtehdpxzyk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gthaisqtrs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtheulfczs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gthfblzhyr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtcmnufmrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hysaishi.cn/gtppudcqku.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtbxucdmmp.html

[E02] 重复字符串
来源：http://hz.zhongyouzk.top/gtrwpevbme.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gtyrwvvumz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ywan-chungtsiang.top/gtqlyygdtb.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtdbshxupc.html

TS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtwepyursg.html

Java: "ab".repeat(3)
来源：http://hz.aizwys.cn/gtzkfkbmft.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtbvmxhyqi.html

Ruby: "ab" * 3
来源：http://hz.yongpay.top/gtjlzwsppq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jianghu66.top/gtzhuucrrd.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gthlmovfuy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gthtdmwuep.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtefrboojz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gthmdhnzit.html

TS:   s.slice(1, 4)
来源：http://hz.hnxiangtu.top/gtidinxyzf.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtsivczrvc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gtewgkhhmo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtqmsdbcow.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtenfodxbl.html

[E04] 查找子串位置
来源：http://hz.kuanghao11.cn/gtzvrznejg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtdanydkeq.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtxycvyczr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtozrznhha.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtcjwujxex.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtjiwffkwv.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gttvtnmpiz.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtnoezulqm.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gttwcxhjhl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nwbrower.top/gtxuqzbqgb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gtriyupjmk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtwlcuzjmx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtuacmyisq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yonumen.top/gtvdfdvjtq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fengsongda.top/gtnaulamma.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hammf.cn/gtmntbvvlz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtiqrjedxl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtphvtaqht.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtkrkbjlmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigufen.top/gtxqiaouga.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydzc1.top/gtedhulglm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtptenrmvw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtsrrngjkh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtfjsphroj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxuanxn.top/gtpltoetia.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258888.top/gttdcrfmon.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxinkj.top/gtykagslur.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gtwgxjmiuq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pengpengdd.cyou/gtpnzrnqrd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258.top/gtqcbyisja.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gtpusixqfm.html

TS:   s.split(",")
来源：http://hz.yuxming.cn/gtfhkyqnse.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhiwuduotai.top/gtnpjcvmto.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.c1oappe.top/gtnncensuw.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtbcvlulih.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cheryme.top/gtemfqbmjp.html

[E08] 数组按分隔符合并
来源：http://hz.yvedp.cn/gtsnmkmiec.html

Py:   ",".join(items)
来源：http://hz.hongshengwenyu.top/gtusnnhwcx.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtyitjnkni.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtuucdrupk.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtodonppoy.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gtukkxcasb.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtwcagzsvq.html

Ruby: items.join(",")
来源：http://hz.havefunace.top/gtvjfufwjo.html

C#:   string.Join(",", items)
来源：http://hz.cucudq.cn/gtwxvpnwhx.html

[E09] 去除所有空白字符
来源：http://hz.xziqi.cn/gtawiqpxcx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gttvpwmxqy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtdycsrzbr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtnxdrrbql.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtenuqiwvy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtiasbofjc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtlazkwzrf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtuelxiyoq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtgfazkeyw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtoaufldzv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtbfetnvru.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.birdmap.top/gtskuqctku.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtseidnplz.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtaxseknnd.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtfecpgdyb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtwglrypbd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtinrogtdd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtprelhfje.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtphxcxosa.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtlugkffth.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtcnkftjvb.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtmxpbdjpu.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtcdazftoh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtckxahzsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gtdrptynnd.html

Ruby: s.reverse
来源：http://hz.ehwqpu.com/gtavtmbsxg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gtbyxauoxk.html

[E12] 统计某字符出现次数
来源：http://hz.xingfuxueyuan.xyz/gthmlvqbpf.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtdvbhhdyh.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtmlgeqhat.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtajdtcflj.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtdlqbiryq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtltyewojd.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtowvzuemc.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtukajkoah.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hongshengwenyu.top/gtenkekfgc.html

[E13] 逐字符遍历
来源：http://hz.jinqigfzy.top/gtwoiyomze.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtjqbtnhrf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtvehzhgul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gthlnzgzpk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtlldoufjq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gteljloonr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sysykeji.top/gtkvjmjcyk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hongshengwenyu.top/gttasgkugq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtoelregvn.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gtcnzsgqzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtoxirjbrh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhaomingkeji.xyz/gtsggsibcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.redwolf501.top/gtxfofwwae.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gturoaibqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtinlmrbvp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtcjkcndkb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pycfn.com/gtakcbfalc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gotoacloud.top/gtkbiubqrq.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtnoiafrsw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtkwyenedo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtjxzvuqhk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtfitbftod.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtdvhivndz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jyoumei.cn/gtvpqlymhn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtmcokopqr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtolqeorux.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtytxkyuyy.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gtavrkmkwy.html

Py:   f"{1234567:,}"
来源：http://hz.redwolf501.top/gtrpnyswrw.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtzfeylgge.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gttkcrihzk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gteeyauate.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtqhcfhyah.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtlohlkmfh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gthynzspkw.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gtrcybxrsj.html

[E17] 首字母大写
来源：http://hz.sysykeji.top/gtcymmkalu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtpefioxpm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinghuilouyu.cn/gttxyivtro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtesbzwtuj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtupyuizsi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gthrxllpfc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pycfn.com/gtuhbztsqt.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gtbsjjdqtf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtojneacwz.html

[E18] 模板占位符替换
来源：http://hz.nanxuanxn.top/gtjtegtolf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtlucbofzs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtmidxjbrg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtemgcrhxy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtdddexzmm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtljpobrdx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtnsvrnxuo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj202588.top/gtegxbtmnj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.meibo888.top/gtyaehuqlg.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtoakcccbw.html

Py:   s.splitlines()
来源：http://hz.fengsongda.top/gtxmoocktc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aizwys.cn/gtqrbrtxhw.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtcscvmweb.html

TS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtcaoewicy.html

Java: s.lines().toList()
来源：http://hz.xingfuxueyuan.xyz/gtdocmhuvr.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhiwuduotai.top/gttzqxtgxm.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gteooofgwv.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtgamwnpvr.html

[E20] 判断字符串是否为空
来源：http://hz.pycfn.com/gtoesxzizt.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtuskrmuut.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxinkj.top/gtfdogghlw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtrgijjbtl.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gthxsgiyyy.html

Java: if (s.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtzjrsyfyy.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtvceppvzg.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtredvqgco.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtptucgwhi.html

[E21] 超长截断加省略号
来源：http://hz.ydjk.org.cn/gtmbddcllh.html


<!-- 参考信息 -->