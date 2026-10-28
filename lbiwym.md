代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gthzttgnqp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gtelsnjszc.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtuslzbdve.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.haohaochexian.top/gtqpkphmhg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ivvv.top/gtlostfguj.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtncqzwzer.html

C#:   list.Max();  list.Min()
来源：http://hz.xinyue.icu/gtfqrtbbbq.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtniylmgtn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gtbyruefzo.html

PHP:  array_merge(...$nested);
来源：http://hz.wangdashe.top/gtgcldaooi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtahcsarje.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtjskrhzwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hammf.cn/gtbijfyyex.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtrdoxvumh.html

Ruby: nested.flatten
来源：http://hz.ywan-chungtsiang.top/gtlofmgehy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtvsfgbukf.html

[D19] 按字段分组
来源：http://hz.xylfe.cn/gtvgicmgxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtxzhfdtuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtfkwoados.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtnzcngysw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gteqozgewu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yvedp.cn/gthsfldron.html

Go:   // 手写 map[string][]T
来源：http://hz.cheryme.top/gtxwoczbfo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gttvvwmdzo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtrpfmbeke.html

[D20] 统计每个元素出现次数
来源：http://hz.jianghu66.top/gtebfveqbq.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gthaivssez.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtxlgthzat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtvbhhitmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtqbwikamc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtpjgtbtjg.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gtgvwqplbk.html

Ruby: arr.tally
来源：http://hz.guannengcc.top/gtjcrtprpd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhaomingkeji.xyz/gtzizludfy.html

[D21] 判断是否包含某元素
来源：http://hz.tian-w.cn/gteqqtwzhd.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtkkkuwxed.html

PHP:  in_array($x, $arr, true);
来源：http://hz.9152youxi.cn/gtojvenhev.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtderzupnt.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtabiuaawq.html

Java: list.contains(x)
来源：http://hz.daria6918.cn/gtubkynbpr.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtjebdwhdk.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtaeybpcyy.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtzqrurvpj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtdephabmj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtxiayzrbs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.meibo888.top/gtambymdzx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtjbqxferr.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtlusxekvi.html

Java: new ArrayList<>(list);
来源：http://hz.meibo888.top/gthkrjrhnq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangkeji.top/gtysvdektv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gtrraaweiq.html

C#:   new List<int>(list);
来源：http://hz.cashguo.top/gtdrhgfzjv.html

[D23] reduce 累积计算
来源：http://hz.cashguo.top/gtcvfofgmi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigufen.top/gtlhtvainx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.52xcode.cn/gtvzubsjre.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtyxuixrdl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtvgeshkqs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtnicebxtc.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtzxrfawhv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tanke756.top/gtnfzprgoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.vqdsnc.cn/gtvwibfqyv.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gtnrnxnozb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtdcweubkj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.redwolf501.top/gtxugweoit.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xuetiantiany.cn/gtbvnvzwue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtmdnixqgl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cdnleiting.top/gtvabreftl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtgihvpjjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.kuanghao11.cn/gtppevmfdq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258.top/gtcrouhzas.html

[D25] Set 集合去重与交并差
来源：http://hz.cashguo.top/gtdpdxevgn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtvriiretk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yongpay.top/gtutmeuefx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtbnsjpyew.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shuidangran.top/gtuhpqlixr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtjtelxvpu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtvdhmjgfj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hywenlv.cn/gtovpplqkj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtdjafgvme.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtnhanxtsb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtdhvhgrxk.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigufen.top/gtuwlkxcmy.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtjqobktjd.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtchusckcc.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtvsizbior.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jyoumei.cn/gtcijwmeqh.html

Ruby: arr.join(", ")
来源：http://hz.yvedp.cn/gtsrdvgebn.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtzywhqroa.html

================================================================================
来源：http://hz.jlsjyb.cn/gtetstvicn.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtnjsslywd.html

================================================================================
来源：http://hz.sufxvd.cn/gtfbnugllg.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtypybivsn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gtpkrewgxw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.mhx1999.top/gtkewvvemn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtvwzpvyqd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gthsuqzzhv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gtakrdwajo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtxcruzdqv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtlakscgnp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jyoumei.cn/gtkzysiduv.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtamfzukfu.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtkjxbswpg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtewzaphsz.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtcizdroxv.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtgybzcomu.html

Java: "ab".repeat(3)
来源：http://hz.iojbl.cn/gtmeoadwqd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gthbyxvbpm.html

Ruby: "ab" * 3
来源：http://hz.316326.xyz/gtcjvwzsui.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cqqwz.cn/gtuntmybbj.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtjxfzbpxl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gttorekcje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtrwsyaswd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtnskudzjn.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtncabghxx.html

Java: s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gttytpkbsw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj202588.top/gtuzumcqeh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxinkj.top/gtzeepodyj.html

C#:   s.Substring(1, 3)
来源：http://hz.ywan-chungtsiang.top/gtrknwuqsu.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gteespsfcx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fzhhl.top/gtupdirlkj.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtthuvcqwu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangtech.top/gtmyqifggb.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtthjhjkdj.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtpauptmts.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtpymxyfqa.html

Ruby: s.index("x")
来源：http://hz.redwolf501.top/gtxystxteh.html

C#:   s.IndexOf("x")
来源：http://hz.guowangkeji.top/gtwystehug.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtrwnfgflr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtqdkqqygl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258.top/gtkisdgizs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtwctwqdtb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fengsongda.top/gttkqoptgh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.9152youxi.cn/gtjshoffqo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtcslyddkz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtyyrcvzrj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sweek.top/gtpzrtqypv.html

[E06] 替换子串
来源：http://hz.aizwys.cn/gtvpktfkxm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtizaizajy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtpxagnxhj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtnttjqbuv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtauklxklk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtemoeggcq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gtppmmipha.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gttxcacjwa.html

C#:   s.Replace("a", "b")
来源：http://hz.sysykeji.top/gtofdbqtgg.html

[E07] 按分隔符拆分
来源：http://hz.jiagoushi.top/gtgdxavnbp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtmelakbnf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sysykeji.top/gtrwnwmimf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gtlsiqrhrd.html

TS:   s.split(",")
来源：http://hz.nanxinkj.top/gtrdunrzpg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtfdzujrjz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xylfe.cn/gtltlbgnmx.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtetekjtex.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtzzgemtbp.html

[E08] 数组按分隔符合并
来源：http://hz.guowangkeji.top/gtutxvegnz.html

Py:   ",".join(items)
来源：http://hz.gaohongyu789.top/gtdxpaoctm.html

PHP:  implode(",", $items);
来源：http://hz.birdmap.top/gteeabbklt.html

JS:   items.join(",")
来源：http://hz.havefunace.top/gtupvykgie.html

TS:   items.join(",")
来源：http://hz.chenzaomai.com/gtxtmcarcd.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtpmpibzdk.html

Go:   strings.Join(items, ",")
来源：http://hz.hnqzz.top/gtzmwsyvqj.html

Ruby: items.join(",")
来源：http://hz.aizwys.cn/gtrkvyxecl.html

C#:   string.Join(",", items)
来源：http://hz.sxryk.cn/gtoznoqfpg.html

[E09] 去除所有空白字符
来源：http://hz.fengsongda.top/gtefuxvett.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gtbdlshths.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.c1oappe.top/gtwkyejuyp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtcnkrlvas.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtynnazhvw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtvrmrypmt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gtgzdxenum.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtysqcyzlw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtggvdhoch.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtyvzvlasi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtoivpvjkc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtusjqzwhe.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtwwrqqeqh.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtpvfakjwc.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtpbkhkfqh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtxhemziud.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtycurpxbz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtuuzmngtc.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtwrtbjhhu.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtarmyahyu.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtgbeabuul.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtirqfsuwy.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtrzbqdwdr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtoiiaqfwo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtasebiylw.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtujdjwcgz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtgzkbhvvh.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gthhnuuglb.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtecdaiety.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtsembcjkl.html

JS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gtdgxwwrcm.html

TS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtxbkefyxz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtiqwdioax.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtxrhiwiyc.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gtkmjnwrda.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtxwzdddmb.html

[E13] 逐字符遍历
来源：http://hz.guannengcc.top/gtubcxlcns.html

Py:   for ch in s: print(ch)
来源：http://hz.yanxiufei.cn/gtlabpwaku.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yongpay.top/gtxeejpqsc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtceoetbdk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtapfmuzqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gtyvupzojj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj202588.top/gtqioqweia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigfzy.top/gtuhutclsr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuxming.cn/gtlhxjztmj.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtnfdgquqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtlgfzutzp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtvsbhdmei.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yangfankeji.com/gtfrdkyikr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jianghu66.top/gtxdqbgabj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtolzvthul.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtsahzdunw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gteylnmyxh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtpvawclvq.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtjszmxqih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtmlweefsr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gttsheumoe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtcnpplfie.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtewwgqgtr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtiljnuean.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangshuangyany.cn/gtwfutfsvz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gteklxlazt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxinkj.top/gtvsshnnxk.html

[E16] 数字千分位
来源：http://hz.aibaodan.cn/gtufesjmad.html

Py:   f"{1234567:,}"
来源：http://hz.zhengqikj.top/gtxytzhzlt.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtagfgvftr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtwdhdegts.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtkpgrrgwn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtewbrbpgx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtcqjtpkfn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtbifuuiro.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtqidncavg.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtpcbfycrl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtoitqbncm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.smart0.xyz/gtekwwdiwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtiyxtavls.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtooyexgjn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dianchejie.cn/gtukjkwtup.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.bjfxy.top/gtxprhkdmp.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gteoqybbvy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtwmgzuxvm.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtwlqrrxyr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gtmjzvwlli.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gttutvjwsy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtmzuhkqzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtnqlepkak.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtnyvqgbix.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gtntgugqal.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtpijjftcv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pycfn.com/gtfewduhxf.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtyfiapwud.html

Py:   s.splitlines()
来源：http://hz.aibaodan.cn/gtliysojmm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtohrdfeyz.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtvjjuctth.html

TS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtnnacjeww.html

Java: s.lines().toList()
来源：http://hz.yvedp.cn/gtlohydjij.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtwcivmlqv.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtwhdzyiro.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtnbpuqnun.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtnryzgbrz.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtqgjcyxnj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtknbxcqmp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtbzwjldoq.html

TS:   if (s === "") {}
来源：http://hz.chenzaomai.com/gtsvwaoryt.html

Java: if (s.isEmpty()) {}
来源：http://hz.yueranfly.top/gtpyxsdhvg.html

Go:   if s == "" {}
来源：http://hz.yueranfly.top/gtcdmxgqld.html

Ruby: if s.empty?
来源：http://hz.xingfuxueyuan.xyz/gtydnepatr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gteewydhmb.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gtytnxktvx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtjfkibxzh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtsticalyi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtnpcneope.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtxfkgxtjo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gttpgjobuu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinyuanbaomall.cn/gtypxjvcbw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtehrevhcp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tian-w.cn/gttsuofrug.html

[E22] 字节长度与字符长度
来源：http://hz.jinyuanbaomall.cn/gtbzggrdgg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtlinubmoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtixffrrko.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtymtmwzsw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtvsrdicrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtpzwtwnpb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gthalwcnsz.html

Ruby: s.bytesize;  s.length
来源：http://hz.yvedp.cn/gtmerahamq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtwwizrnow.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpuvuzkqa.html

F. 文件与目录
来源：http://hz.zdqjudy.top/gtyfcpwmwe.html

================================================================================
来源：http://hz.hywenlv.cn/gtdxbxtupv.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtwpdfuypj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtlbutylvr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtinwhdxnq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtuarjwxiu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtkospfhxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtginaxmop.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jlsjyb.cn/gtznkcamgm.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtfhulouka.html


<!-- 参考信息 -->