代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gwvzqoejv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/ghuokbxfh.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gxwsnndzz.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gpfllbfcx.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gqphgahxv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdfixkqaf.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gvpndyxxk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gdpigaozb.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gleqbdvqr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gcabahweh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gsbumuvnt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/ggfzzeils.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gnowgcwjs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gosdttiqp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/ghghzklzn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzvejznfa.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gripqnnah.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyitpukgg.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gvpbbrrmm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/ggqkyajey.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/goyzmbjcc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gfywclwai.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gnwxigqnv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gqxullmcb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gbhjdohzq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gaqqogdqj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gqyfxmhzg.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gopjoajvp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/ghgyoilue.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/giqpxhbfi.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqqtmuyac.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gpwowidww.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/ghktuxodn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/glhhcyzqm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gruhnzajo.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gavpdfccg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gfbozhrkk.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gvhgjmjxw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gabhellqo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gvqlnyvqm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnaaufeto.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsyjwfpan.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghnilblxx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gqmymmbst.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqrffwnge.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gdymsfkja.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/goppvriws.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gphpgcpwd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gsesvcgxv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/ghawxtkkm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gyarirfav.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gzcpfskby.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwquxstpp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gjhfxzkyy.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gtwlcldjs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gesirvlto.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gubjzmnpm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcxxpamqi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gorjtzakj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/grxprvxee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkgefeeos.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gksfbuedg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gpvwkgbph.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/glwwwjifp.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gunktgthl.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbubegybs.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gbqbautlo.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gwxqrgqss.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gsiglyalb.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gnfithqur.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkngfwfve.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gpuacnytq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gvuiopimi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/githquevf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtzvchkdu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gubjlbqeu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ghfmyjudq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfnjoaaps.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gumtfxahn.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gwrykjyjo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gvbzotogu.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/golzjoetv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gsdllmtbq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gpffcnzel.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/genjvuuuw.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gcikkrgkp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/ggckorljb.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gxhoxjmgb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gqueabhjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/glcrzcaux.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gwjahnqry.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwftzfwcz.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gwvqlizsm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gjvksdltg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gqpsrrheu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gqppucpqd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmkvsfbix.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfaeaably.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/galmgysbs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gzexqlcoo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gsqkxhfvk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gxbfrvczj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gpolnssbz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gyuktkqer.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gwcgjdlyk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gventnsdm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghxxlyfil.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/grfptuaxv.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gntvjqfdi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gtaussiih.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/glilvmmvc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/goewjeiqu.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gqxmlkebf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gfsgptbeb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gmteujlef.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gcayiabwo.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/giafezstj.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gfyheopwt.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/grbmjhuax.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjceehhui.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gekxftvit.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/guvgvjjsv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/ghsqqxzll.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwegqpfgl.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/grahfhgas.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gyzrncgjx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gumtbpcfa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gkuucozjr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/guikihsjv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gmjgizahv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gtpfdysuu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtyruqrdh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gvyfcssvq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/glgaxluhe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcfqzmodh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gzppbghjq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gizgkspeo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdetarskj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/ghfbfkcqo.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gzzofuoos.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/guietbekc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gcqsvipel.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gnibhzusx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkvvxkkoz.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gtrcgficy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glcunxdkf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gdsalcrkg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gncrmnqss.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnlgayylw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gcstqklps.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gpemlzvzg.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gptxgfmfc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/glhsmohra.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/goiiwvpoy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxygzdxiy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gbfydrgvx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gijjfetei.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gglickods.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gufjxkqhb.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gkveasblt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gwcwhjzhl.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gviczfwwk.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gzoqyuvro.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjbiuzhac.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/grbmffndm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gwwfjnlqz.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gujzpexgw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gnnyqmooi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gisbwppif.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gkgvizqwh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gnfreojcu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gptchtzco.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gikoppgdo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/grjknwytp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/ghdtdcudy.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gftgatxrh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gbobtubvw.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gnsesxaam.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gukppshyt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gkabmiwib.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/ghqijeuyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gzfzxgswm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gevanbsjv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gdhhvzfop.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gbubngiau.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gpwkwxqfw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gtkyhiury.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gsummilia.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gndejjmok.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/golfvverh.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/goktialib.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gpfpzdxsw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gkvgjakou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gaavnbcrt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gvnsykqfd.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/ginjgboon.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gndmtmxsa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gdukpafoc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gbegjidbf.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gjknglfhe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gpwdwlkmx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghnwissxg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvxsfahue.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gczwpbuld.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gaqigvpsr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gzykirfox.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/giqvphvmp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gyuudxdgd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gpuhabjbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/ghwwxjyai.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gwrfktpgk.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gdaxjiwwg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/giaeuoevm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gddcutqbn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gecmmrfcn.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gzohnmvxz.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gdpkbuusm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gvkgfrsya.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghdmckrxr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gomiykfno.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcbdaavur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/ghwoqchcn.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gjfnsgmdk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gicdudxzc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gmzakforg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gvhyafhug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gjwignipi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gwstsaffe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gifkgbyuf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwwauyzza.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gzesjqxci.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gkcgmllav.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gdtxaahzr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gppuengie.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gndwcbudx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/ghoxprnqf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gzamrmfes.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/golnvohsf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gtldsczsj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gvkxvlqan.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gpjmsdlji.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/ggsragfmk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gwejzeytd.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gxddffihw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gizczbmal.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gldvgkefq.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gshdcxzyo.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqscwvtbx.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gnpctkrvt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gnucybsuy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grlwpxeab.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpbadroon.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gypqcchms.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gakpgwmil.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gguxdenwl.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gplahuhra.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/godeqrhpp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/garxuamty.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmubdhbut.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gaqusbuqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ggypgadvb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gnlqsylnr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gwjvujxie.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gikgmvxhm.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gbkjhesqc.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/goprepabm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gxbcscufe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/glgfvspqy.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhptdfm.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtyzmdjll.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/guaobzoyn.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gldxnonkx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gtsssofxn.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/goteurgtl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gkdwwqpdj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpcfpfvea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gjreeozri.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gtbkapeek.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gllxvfqse.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/ghlgyzluj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gwlhmdxbp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtjwzuhlv.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gbnnmqxmd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/guyqklaux.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gqmyjjztu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gyterosic.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzgyjldhz.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gziyvcjgi.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gzpekwset.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvynpesvl.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqprwhebo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/glbqjbgyv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gyvrpmtxu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/ggyxkmogq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpnrfnqhi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gkjdebisi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gorilomno.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gshdyhtrb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gnzwrgxan.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmlvwpepd.sHtML


<!-- 参考信息 -->