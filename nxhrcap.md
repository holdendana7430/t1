代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gbefvigfa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gpcrwfyfd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ggpbdpdri.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gonvlacuu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gifgwzvrk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqmopgnht.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/goteyvksx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gfxtmdnmy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/goagknhtn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gqticpzdk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gflqhrfbh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gpgwqvqrp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gpvulpjbz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gjbweikyh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gwtlgppcw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gffpzhbaw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gnlugkpzz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/geapzycvr.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gflcifrlo.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpvrqrker.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gphutvntv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gbvpnmvnj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gwkgvoqph.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbyhxdbfb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gjcnczlfs.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gbtifhory.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gzhvghlod.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gtvwjjzwa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gysrjxufr.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/glpzoktji.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gvthpzyuk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gvevwkzyf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gvtznjamh.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/ggybhjxcj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gdudpmipu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtzdeexfo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/ggvtlkstw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gidqpqelf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gepooqdso.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gqerqppuw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gwnupxite.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gsenlieom.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gcqmkektc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gvxpmhmyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvpauybrl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdtmvcmmv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gdazkqbrq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gfvkuqpwr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gbezhwhtq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gnefxbtca.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gatxlsdcw.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/ghcmyygpg.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvkckpqur.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gulxabrno.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gjakqyfzp.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gzxipiice.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gvxdqjckc.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggmvvfswo.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gurdiovjz.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gdvfyeoqt.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gvebgmnga.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/ggfzsaciw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gwokqzcrn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghuvgjyah.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gsibykhzy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqstbdlen.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gylqnednd.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gxkdirsci.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gfjllbvdg.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/ghyrkpmuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdodccpn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gkxdsajqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gjqgyjypj.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gyvjnmdqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gfyulowwn.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gecdrvfrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gwdvmyzfm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/ghsjantqs.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gpnhoobsx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gkpidbkgs.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gqzmceujh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gvrqmmomz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gqsamzmoq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gkqjgsqyz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gakaxsisz.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfewaftet.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gncmtwnqk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gjzwskpnd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gajvtygbs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gspedkfcg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmagnygmc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/goplunzyw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gmkibebfm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gchkswuxd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gzitgjzzt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gaxhqimfv.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gqpvvsloh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gcdwrytup.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gzpyxlyzj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gviuqzbrs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gbevbeyqu.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gvsvpuyqq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gcebjxxgm.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/giyjxnmkx.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/glccgagsd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gqpwuotjq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gvqyyerkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwflepdmz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glrvetsuo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gufujhoqf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/geupvhndn.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gseqzlpuc.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gpxodlfjn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/guofnsfku.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/givolngmv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gtonncbts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/geouyjrcs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsrtkyvfh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gnddrendq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gfxwfjcma.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/grxykxnst.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gzdklrqnc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkujxntpw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gkvygsoma.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbbojdsxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjpdjehkj.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gydubxhaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/guobbpbtp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpeignzyb.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gevliyroq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbxgnxqah.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtdukcrey.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gdlwibrql.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/ghbxpuszj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gaalytpif.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gaxrhukge.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvbmipekt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gftrcbike.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/grwugspps.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gdiuayjgc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gnsefuyeb.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gfairtzul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gworfcwcl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gwwpniyxo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvcoakmfc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwhrmyltv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gqmjoqife.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gblsoxtwe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gtzlffuov.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gynndylyu.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gbfleqopn.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gsglobxue.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gqyhsmtdr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gbrpybdxj.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gnwvhdcpy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/giaaxqrer.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gitgywhkm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gvfhtusyo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gkzvzqvgy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gdticripx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gceknxobj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/ghlsdxwir.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gewhhybgk.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gxmzxbtst.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grgxskrlw.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gwmuuyesm.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gvhdbqpms.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyiohfrqb.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gnkkikpyi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/giurkrpjv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gvxivxtcr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gpqsnheec.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gefzsngsi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gifgmdkuk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/geeybrpgq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gpxxxucif.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gzjjijftv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gjeeinboi.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqicafaiv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkmsogoll.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnacqpuze.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gilltayzd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/ggkzsotng.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gmkyardzn.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gmjuklugp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/guffaelxy.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gruajqksv.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gacpkvazm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvhsllcmn.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjnvgnlgr.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/geliatfrv.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gixvshljm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqlveudtl.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gzhjmswjz.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gzagylkii.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gnudpclid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtlsekahs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gawoheemx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/ghhosscng.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gzaemxykw.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gbwpvnfjv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gkxokqmgu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gqjjqbsbq.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gqmkipilu.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gpbdjewgo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gkiszlzoc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gesyesyyk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbgpcwwhy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gkpdccxiz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/glcysaciq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/ghybjjtin.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gcydljiyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gtzzvuxgh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/grmzxgsiv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/giykvmzym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/grxgrldwg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gknjzlnwy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbcraiflq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gajvricff.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/genhpygon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gmfffjksi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gtfwkguku.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gswiwhhvr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/ghikjxxgu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gysqariks.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gwblufrry.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gsvdceqck.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gufcinavr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/glxrmutvi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gohdjqhnc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gcostnxgu.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gxaquczaq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gwrcugwmj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gtqrzcxmo.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ggmduuxdk.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkdnblqvx.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gfhxtiuph.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/guamqlrgv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/garafarud.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gmhfhiguz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhluzjlk.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ggcdpdpuz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gksaaogwf.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmedpbgne.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gpyeixvec.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/grmlpbsdg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gctjzfmku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvxzsnwtl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gaeolnnrr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gjypheowu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gdynjicwn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvyitlhhx.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gbmszggwg.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghtqnnmtz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gzlavbuvr.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghbtugqox.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gyyjdbcvj.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gqjbedalm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gafnaixeo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gkfxxkujf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzckryjnm.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grwnawxuq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gtkdxidue.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmxrwpbwy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvhbnjzpu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqdghwegn.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gvmvykgbw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmyiwlkwf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gwgcvgowd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gwohbmhdk.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gkeiipwai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gyxxebriu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvweahztb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gbyhtuhgc.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gwjbevxau.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/godullcaf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gpzvikjkx.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdpspmrye.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmmbrlgzh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/ggrbqrxtg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gcbccrkgx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gbbvzvwiq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gllsqtgik.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gsabxexru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxvmrzyhf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gvspwfzct.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/ghxlgmpjd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gabdaqobg.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gqczrysyt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gpyjmdufo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdizmsrtd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdmmgxfnm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsllvloyr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbebxxoeg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gjfsaramx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjhhkpezd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gejnvswcp.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gwurljkrr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gqjxoeljh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/grwyyzqcz.sHtML


<!-- 参考信息 -->