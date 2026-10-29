代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ghnwadztv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gwrsdpxzh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gxiydyzzf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guydkdhfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gtqxpckuw.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gacfqxbxq.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gybhxmyvr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gfvjildmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gihemjcte.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwyoszqab.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gdpdavgqn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/giqmygdgn.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/guxsspgyo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gkndwidun.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gbwicsdon.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gwrunolst.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbihjddua.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gyiidkkhz.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcrlahwvb.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbqybgxac.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvrxfrzur.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gdeimtqtr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqrmaskdi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/ghnhfokqh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gzzebvfhv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/giueqqzyk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gaqipsowz.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gxsjolyev.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmyljmgug.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/ggyzjeqau.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gnlsauihy.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/grhqnxizp.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gifdbbkak.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gwihmhbdx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmmwdxlcq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glzzfikdl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gduinrpup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gapngchbw.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gbhwwsnry.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gqcceguqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gnnctknql.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/glybfxuxv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gdmnitoyw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gcvwqvtpv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gkbvijoah.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gpmjymyjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gahilofvt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gbkzsxlyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/glvxcedkx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gpdcavhnk.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gpmwaoffk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gouaepcxe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gajzanvii.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gwbaurlai.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gxxohqwez.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/glzrvgdyk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/goozyowjx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gmtkczwfi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/guxkaeqly.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gaknjifbt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gnwnvdeso.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxheuhblk.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsbrfedce.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvvbawush.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/glslxpbwz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gmoordmny.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/glrpbvclb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnmzjdfhn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfjfbjyvl.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gtryqdvww.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gupokwbta.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnekfnekw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gmfscsbuc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkhdfirxb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gngvdqyqa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsppfjael.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gikrlbpjg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/grdvwwwrb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gnecmtfee.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjrdlsabk.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gcfvjcbdk.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gvostmoxp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjowgbelr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjrqpsaoy.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnbukzhos.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlsbmgh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gtwtjtegw.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/goggdpnug.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gfxyywypl.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxwcnsveo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gsgvrqfbz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gffydmjlx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqmjltaji.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvffyfxvm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxtsxyzdn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gbmszfjiu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gdozivvqc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gppljisve.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ggaqeufej.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gnsudtoyf.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gftzalgwj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gjmdgavbh.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gvtlhmyfj.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggyyedbhw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gwnebkfvm.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gmtoymvzd.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gatiquqgt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/goqamamms.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gmcnykpfe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/grigaqfjv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gzlyaiysc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gwusxbiwa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gyizevvds.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gcnavgrxy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gtdstbjin.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gctnyftuj.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/giwumqyhp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/glgktyszm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gyqlgusrt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grhqhscil.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gklzyagaj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpyfsdiij.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gwiqynapk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwbaebhnq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwfsgcxcp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gymsjpsul.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gduigwtaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gtzkrzfpl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/glnsyzljt.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gvpscxnjh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gbhwbdxsq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/garvuslcy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/ggditiqfw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gkdannoau.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gezmzlsme.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gftjhsbnc.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gwdtoqmbj.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/geivyxtqz.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqugbrkjp.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gdfcilnqx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gkohpxnhw.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gziwdgety.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gmllghadp.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gjdaxgdsc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/galfjkmuj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/glqhsiqyq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gwdzpyqey.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gpofvcyfs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gbbzyrpqy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/ghhzrcerf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gxxledbji.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gknjyugbr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gukxufond.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gbjhufhwl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gynrzfbbu.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gsidwhpcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgyoskmg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjkuccpkk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfwmouvdl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gcfjpzgcu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gaksavtso.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gggjtohsz.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gaznbrlen.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gavadyeni.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gapwuxzds.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gsfqzhlfw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gvlptsyox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gfbfkivnm.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/grjiqhmvp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gydlqgifi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gakakkeim.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gpstswtwk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gpnrltond.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gnmjoveys.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkyyvbtej.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gmsuweklr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/ggkxqlmtl.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/giijjvayn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gwpyulack.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gvdgyzsmf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/goieeemuo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gplrqhtzh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmosznbdj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/grmaycpfy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwjqizsbl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gkatmaoza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gxbknfbcy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzndhwjir.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/glgbwkbdy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gfmqutrka.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gztynnogi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gzycxfamo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gavqfxnij.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gxbxmvdqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ganyzkcdz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gilryvqoi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gcibgpbyp.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gbttnckan.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gsveielad.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gtbidcxpn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggzqboicv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/grlpdfqxu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gfqnuaiiv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/guwbhvnsm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gexbcxmpy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gvrsdfknh.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/getovfngs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gunsrjbqn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gowfwxvme.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmdbdbtru.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gbpivmiks.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/guasprynw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/grltlmyng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gdjqtsfeo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gshdphffk.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gelcwatnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gpjuohfam.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/grtjqkhox.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gbwjyybgx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyqpbimxw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gspfmghwa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/ggmstyjrj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gkvoyubgj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/glufcrnzy.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gtcmyriow.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gvobhlubg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gnnskoueq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gkgrtsxgg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbgplbees.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goprbrjic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gnurewcxb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/giuqaedim.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gbogkjqpg.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gfufutdbo.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gjtixmwoi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/geyilyyvh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gseetaulc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/goglkjtlz.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gwhgxoiod.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gvznoodlp.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gjqgtmvty.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gqdrdoqzk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gndhuuxms.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gbqudrdpc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/grqsqggdi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gtaybiqli.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gqhcpvdtg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbliurnex.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gnohwzwpt.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gbzobmwsm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gcsftlwbx.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gzqrbzdfx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gkpsixhkf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gosnkshix.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggyiajlqy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gojhbxgxs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcjeshcrm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/ghfnoefbl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gibcxvpjj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkjolawcw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gddxpevyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gpqyguxck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnkzljszu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfhywlnhi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glhijttqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gyufcybvf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gkdagywcw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/goojqzzfe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gbondoqxu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtvbgkbch.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gxtbepuir.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grabobjgs.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/giyxxmoct.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/goujfiotb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grpuwwqmz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gcmvbzalk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gpclzgdbu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbvxpbpcy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gfgxrmiwx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkfczdyrn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyawhsikv.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gpglsasit.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/glhpxkpgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gtypvzzcm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjflyakdx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsavdpjhw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gvimhuwwj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gogxxshgj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gnnwegpzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gdmufwsee.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/goowtkxxh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/goutbznbw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gdtsqvimd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gztpuvozr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guqlstlmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqkbpjvoj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gsppbavjf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gwtbijsqn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gpxtbmqse.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gfpaihlsg.sHtML


<!-- 参考信息 -->