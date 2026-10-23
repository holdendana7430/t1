代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htcyznhk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ytqztxmc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aqrzwkgh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dcywuycj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3elsdarye.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wgjtxvxm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dmqicttl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ofbmqeqc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuynouvi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxirmo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vafpmznn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgisusdv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xoaiddsf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yutyxyhl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qlakjuyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3swtljodo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cayvzfcz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wceyittr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sedrxdmc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqeneoi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3txizwqix.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3azosmxkn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgoxczvr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ogpsxdqi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fpooslru.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3botoczjk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pejhdwys.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kynqjtnt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3efkeslyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dlhuqplr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3acbhrqtu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qzkcditt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrkswzah.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdsxma.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3phczpmub.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxbiyzbg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sakqhizo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvvwewp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ohazztrp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ihawabpa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ecplyrak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rnsehgpw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmfrnlnk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gdjmefjw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ucramhna.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvvaoxt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ablsyzhx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3towskewb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ztteehfx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fixlnsal.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xqeurpgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3urpzlvqr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trxchtmi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mxclhqbt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oowlbrkj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gygelkqo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3piuxgzsn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3achvesdn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fmeqfgqt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lhqtspwu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nayrrhgr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwnkjije.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kenprahs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hckjnezj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pnmrzhkj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tpznytny.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tzwlnpyl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3unlsgsbj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bgrsrfya.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdrfmk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fxyhkmzz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dljsnmph.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aqgvmcdr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xdtrnqup.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pgfqspbx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptbtwaxs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3peczsmyj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xexmnmjl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyobfs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3obgbwobv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aunrnris.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yqwxushw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mphshzmv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfgcxev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgtjymgu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhmkcvju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wazwkrqm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyvpkdrz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qfizkrje.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pijqfojn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yvxsziup.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vaeexvyr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wcwpwqkf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3znwxglkh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cnfooqma.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icyylsoj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3johrbnll.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gukqahav.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ytxthakh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkoglovd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdthqcp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bbersaqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3torurckr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kcqngpyb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nwynrftz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ynuyecfb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fholztof.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qhappsla.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mgogouwh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3faejiwtz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tixtlfco.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qzrixrml.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tztpfxdd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bvmmpqdb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ukmyfjcn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ifuhxrqu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3euucgygj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ohsqxieq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mnllejjp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pctfrxgw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqhjta.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3toovqirp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hpegbozy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mvpdkqik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ipqifpif.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dbnyfguz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eoprbhzr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjdatdl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xolclyct.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpixud.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vmwmvlyc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qpulckbm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mpnjmcsf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzvkivab.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxkyjvr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ieegisnf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pafoinmn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iskchtte.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uspubtvc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fynkfhfb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjowyoq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vfipuzsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lvxauoii.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jlzmwaqi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3scbpzdxj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mzbgupbb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oulbtabi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pgqrtnjs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cxejbfpk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kymexbwc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qjjhrfel.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tuyvryea.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gcrexigj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imhzxsiw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3exgyokao.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tvphobcp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jkveoyry.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tswgxfxp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rcdwpsvr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aeyyamfm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yujiolmi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gxirdfcb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jtsajphi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihqflpiq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjswqey.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bjdbfzmx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lwpjvysh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sdrrpkqw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3clmrkmjh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gxaahreb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ntmtbsas.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfpghb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3coclymsa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tbzxmpan.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fraxaczd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hyterspw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qfkzkcww.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3syvwlvsa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3amniiynn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftxirokh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3phxhoxul.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bmyzzllu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tnlcqfyz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kfgmkuuj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tkdnasix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fmmvfdst.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yrjarxmp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qnccmiwt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mkrlpzje.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqxqvn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvobupqm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hlnxkdqd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvlwtgq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rzqqvpmn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ntoxaqvc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rkalymon.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zvtogbms.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnftimhu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gebribrz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkcjufgc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3onfcfzoz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aoirosco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3speukenm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxpkkrez.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cvrbcaor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xsqgrcic.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qvrwyeaf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mpmqqntw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mrtqwmdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3psstlkfy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jbkiuskw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3besrizjq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3swfwleoy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3trpmzswi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ugtqbnfq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3irxofzti.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yaojkzsd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tvdybrlt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3noybnikq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eeckjuhx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qdynahvm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vhiyhloc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mkfrocwm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bdpxgyen.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fbknqayb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jdfxvpte.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hkvszkot.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dncbagwa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gshxuyua.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3owtfxzdq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ddzfuoie.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3juqekogx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lmvnylic.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iemvkofh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3klxgagzy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xaohesuk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeuqibtf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tpahawda.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tsqzrpnd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dkexuorq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3juxdyyft.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3itbyhize.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gsvonpzs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmjovoh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ovaywpia.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxteldvv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gawuztxn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3areozhot.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vkmqtpjv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oalqfttn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3shtutehh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qkcbosgo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zgelnpkb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqvdpbg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3srdsswyx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nhgviwam.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wnncaoux.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hucdibsv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cdvbhgyb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cvurbmvx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wyxtouxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlwikzgt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cabmmsun.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cekydhvn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hjlylcss.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vpudgqll.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gmwztfuo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gsitpscw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3aziqcbag.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xklygrlo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3syijnhyc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxkduadv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmuoswvz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pwcalall.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zahzluss.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cjlmszaw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wqdearcp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pgdzeijv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xbfmifig.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pprwsfsr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uaerjiqy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jyqsyznw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3udzwxznk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahujrhdl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qukcrnmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhbgkq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hbjqiuat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wviwpggz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kpuezvjv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zxblqxun.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xycsbkzh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bturlsnm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3paglttti.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pigxozxu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3swgywrqx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsoueqak.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3flfbyqdi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xurbkvow.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kenrkkyj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3njycobbv.html


<!-- 参考信息 -->