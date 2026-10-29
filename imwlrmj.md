代发 wailian999

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gmprtxvgc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxymiwdpx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/ghtaleewt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gybiolkqb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gmnzkddjw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gpptsspeo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gcqhmhmcy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ggmfhfjpd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gsuatrlnl.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gcbaeblbe.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gfqfljolh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gxxqfutcf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjtjhhzsu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gthgxwwhr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gibnwefza.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gsqgnwopl.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gqeewvnhf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghggcsccz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/ghvuhjybq.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmeaspvvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geqexzsjd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvunqlrm.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grsppisyv.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxpuaqqnu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gthckrsbe.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gelixyiju.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gopbyefkc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gpdfxccpy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gparxkrat.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gycwqlpbr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gbcfudrut.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gerncfdzo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gmbdqmcar.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gqlekdqfj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gxemstojv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gtfyyrqcv.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gzbpjndkf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gijdnnsss.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gvvltqris.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghwxiqmid.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glsictybz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/grzdxormu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gdvidxodd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gdjhzamhv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gtdowvyqy.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gkbvmxacu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gyuvxsfzh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gaoiwsahh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gcsxaqccp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gikoqjozq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gfwvwludw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gdxpsilkm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/ghplrotgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gieacheln.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/ghlicvrud.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gvhdkqwtg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggtotawlz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gverwpzrn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gdpyhegkp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gmnxwxnrp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gyuqvgfen.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwezdpglb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/godbljnbu.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/grtzoagej.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/ggvtzmmsx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gqeblkjnt.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gixzstgja.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gtxvogssz.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmbgdtkde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gssicrmra.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gagmxvtzk.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gkwebjpfm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggjvlapna.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gflfeeann.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guhrbxibf.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gwejmscsp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gfrjdfaps.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gahszurno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gmmbmcmbq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gtmqolclf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gfdrrpnpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gmwrlxwrl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/griytgzyx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdjnimixq.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gvldomhkx.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gepjfmzfm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gnhlbspnu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfbnycped.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbpiixqfr.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gebgukigf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gqtuqavkn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/godcsoaum.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gqbavfkch.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gdevlbjis.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/glqmsdcsf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gnqpgdfmf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggjbgkjzi.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gzpvxqpub.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gzuogvqjd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/giqinikqw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gdwzecnmo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/ghpwhmvld.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/grxjfqvhi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gatkmmsji.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gtnnazskw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gjcutmvpo.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggoqartvv.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gowffeuvo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gntwkzfye.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gndrvufzs.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/govtikcow.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gwipqhaji.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gyttakfvg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gyhdookul.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gcjnsjegl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gamymmepb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gyghnmnqz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gwvtlvrng.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpyyxxksx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggyukmwcy.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gxjshdbfb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gatpaguvi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gemuezszo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnqvnknue.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkytbnrvz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwudsfmhv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gcbqbusek.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghlmgiweo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjpcpxpat.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gbmhgqxyx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gmuqgjmnl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ggqxlkitp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gjajthelb.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/geyobqqjk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gxjhbdlas.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gthfghevt.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gywkljwtb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/geiieslfj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/ghtsnsrou.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gvfjntpol.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gyokbecsl.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjrzcxa.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/glbbvrkte.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gbasllcax.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/ghlnziblf.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gthruqdfs.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gztmtyqgd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gonotmntn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gomoaweap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gobokvheb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gtspkwrwk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gpsrhpdxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gbzjmsdbf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gbnfmctfg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gvrtlpvgz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gzktutvjt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gfrunexyf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwlhgultf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gxirrcuzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzoeaplgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtpjlduxd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guxxuskhf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gicvqlmum.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghxtahkts.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gsfkpngjc.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gtngqayrc.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gphyozjzx.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ggoxflhcm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gisubvxcp.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/guubursng.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/ggahaazlc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gjyuolove.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gnnlpwqoa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbhkiwtgm.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gkmxngoki.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gmxieebed.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gilutasor.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/glquckhah.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ghujiyukj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/ginshqrus.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gblhsqlcn.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gsgqjlxlm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gwnizzkym.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/ghisgzxdd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gappgvedn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gqutmhpvf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdrfsnhcy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/glqynrwlc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gpiyeqtzg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/getrpxevo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gkgijttyj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gzazgpphc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/guaapgasq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/ghicrfrvx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gbyntzpuj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/goviukswc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gwvlmesth.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gyalxcyge.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gpljzzxqs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gadilohjg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqmbdjvgb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gtvhoqexo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gwjicvyhx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gxbnntorp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gijaeltft.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gffifomjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gwcpsurhc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ghytpcmyq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gcsuxpgzx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gjdukmcol.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gccelhxqx.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gcijfbmmy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gyvczssdl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ggsskudrl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/guxmvcvqq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/glyjmtrrn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gqiftwevn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gffjevlbf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gmjkztzut.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gecznsluj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjeezyfl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gcgktdedi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/govyltrik.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gtabdgggw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gotbqmdke.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gqbilcxbf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gsdbprlkd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gmhvtedau.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gadkjeicn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gdbxcfjtd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gobcklbbp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvbkuzdld.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghspwuyot.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gvhbumxjv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkjfmomns.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gbovbmixj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/glfiotmon.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gaczbnphl.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gpaonybpr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdhvycrkq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gastmwdyo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gngeigjzz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqpadwehx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gzglxxpcb.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gsvyycrwf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/grpqpuumt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gcwdvvqvz.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gggetdvyu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gywvqeshq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gsmzwzwxs.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gyptfpoyo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gtzefdisa.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gpsauteoz.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ggsjezdkn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gasbsazms.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gmbiwhfti.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gporurijw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gehmtziuu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbmwgurcr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/giwawxpcf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghvztnwtw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gatidelhf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdidrskrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqiivbjep.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gnevyydhe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/ghawszorz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gxljcohou.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gefohdudv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqntsanbc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gvgikwtmo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gerucyakx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkokplwue.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/ggpjjrzlq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gonjlqbgv.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gdwwudmla.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpaloiykg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gulikagrr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/glawbluiw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gplwvtooc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/ghizlazmv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gzdnjagpk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gasfhhqew.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/grjwbntxh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpqqsrwrb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gphyovpjj.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gbdqjywwz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gomwkzesh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gunenfswi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gihrciwes.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gxeotitqj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gtulmrkdf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/glpgdjhyy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gppynqgtt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhgbojt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gubvzedad.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/giternzym.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwedeoryx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/getcbtdhi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gketvermq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/galqmbpzx.sHtML


<!-- 参考信息 -->