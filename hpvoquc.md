代发 wailian999

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gpdhnwxfq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gpyydrsvt.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gvrrzllro.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gkhmltuap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gmrkjcehs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gmgucuqca.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gncwcbmga.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/guzgqxpzf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gmhxqnuxv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gwxxizkyw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gyfnjdqyr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/grbydasyy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/ghvrvtyhy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gxovmojqw.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gpyitrvlo.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gkvdvsmyg.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gkanmptlz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gadnwcnjh.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/glzytjuda.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gilmuychz.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gqxznfjrw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/glcygdtin.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gsobqmdtw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ghguhhbdq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gjkyihboj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyrziflwh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gassjcboq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grajbbmqt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gffpbqaos.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gskcrmeqf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ghgafkiwc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gplfzltah.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gcagdvyyc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gsikvcviw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gqlgofiup.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gyhywjuod.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/ggxcrmjap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gdeaekvbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gmcpjxilk.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gkzvqfyko.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gpxsaosux.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtsburjmq.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ggjtfekrn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gomhfmktr.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gfplxspdm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gwmofqpgl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gjrqxercg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdmirmsme.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gawiwjnwt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gswkairaf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/guqwwdzdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/geviodnie.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdlhabdqi.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gurjmwcxq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gdjdgihhu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gjdtxsdch.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gulxqtptd.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gumocxzfd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gtwhfyzhu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gufvfxdwg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gvcontowd.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gvpouetwf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gnvdomnxg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gcnrinmrs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gkgxoatgd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gqudcaepn.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gntywfzfr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzznxxaxa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwglqvwep.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/geyzogopi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gdgrfruev.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gzwijbbxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxaljwaxh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gyhblyxip.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gplmlqigc.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gbduzkcgr.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnocllnnq.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gvzulzkje.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/grkmunmoj.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grdboegiw.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/grfecpexf.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/grhlfpkrl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gnwbcjlrx.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gpagjfkck.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gtqmgzfbl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gsqzejnbi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gbfsewlwz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gpywwvtgu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gtquiohxh.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gufwzqgrc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gezkwdyhg.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/ggtfosaet.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gsrrxhoyv.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gjbtttwyi.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gkynyctaj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gdysmtuxs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gmwkwyiai.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gsceuachu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gtezaerbd.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gqwykotlu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gqkvbozdn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggmauubdb.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gimwpopgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gindorqbf.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjclutchb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gpkjqlned.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gtajunroo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gdrocdqsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/goqmotbom.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/guqhlrjqb.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gjotbjaop.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/ganldaxtr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gramasiiz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gniqptxmm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gfqrpkrmo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gbagjzvsz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gdfpgzuwu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gnrrgykcb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/glcnwlvrf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gkfpgfwve.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gaqedgnso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gxgmzjvfm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/grvlwazxx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gaqlzkcbt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gbvwurawx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnqjhdlzh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqyeikqtz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnkugiquz.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gzscwgypr.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gbxfhkpgx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkodhdrpz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gjklplgls.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gqzdgtrfv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gkopfxjos.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gruumvxsp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gznlgbdhf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/glcaqkoxq.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ggcjjgzwt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gdxdowbgp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gygkuxava.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtlcdrqhe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxoprjsir.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gzbjviuss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gphzlokjo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gtkkpcqxt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gpzylttrx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/glmdxkgku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gilehqrao.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gylpzkoav.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsavevflz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gviweezji.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gqxyzjcme.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsceluacz.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gowqadxrr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gdljbamfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggoauhgkd.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gtgsdbgnm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gcosptqqb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcqjiafuq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gtgbqigxh.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbrzojyth.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gebddxxqg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gymqpragi.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gkflpyije.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gzjcxpmlx.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gvobdthuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gggafpkxo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gcjdceajp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwdbqnhar.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/goybkkxkn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gnmplgggn.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gbmuhmkdz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ghtocucnp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gaflqmibi.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gfjtynlbk.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gvhqzfjoj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvelqmxur.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqqdiynvg.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/ghvapgobc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gmvkqhxja.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grwqngnhs.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gjtwvyfpg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gmalexaee.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gzpueqvdw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gtprlhtah.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gtmzmkiso.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gtfvazfoo.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gluseunxl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbdjiytxm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/ggyevrhdi.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gdkymxvoa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gduavugvi.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/grqfuhfdt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmbqzili.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gpfreyrsd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gfcjiooez.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/ghhbwivlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/geyumpltu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gblbwxvbs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhuylnu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/goutntizm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/ghfhmwlmn.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gpplezsmw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/guemlmboe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxqfjbesf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gnkgsfvmn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gnwclisjo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzkmmdwkf.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/ggvscqdap.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gjhppovjl.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gvcccbbxi.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyrjdbn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/giqldolmb.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gwvwfiwbk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjptmqnfo.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gjajwxmvl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/glckybskh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtphkchaz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gjkzxsmmp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gqghxaryw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrygbpts.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gtulcxexj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvmtbvlct.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gevbkqnnb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gintlgfjq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gxiwilzrn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gilxdkmkl.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gysgoqoqn.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gvicxtjpr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqewjamgr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gipqtvhfs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gelgrpjed.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmlgdiuky.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gysineiyy.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gxxsmzcja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gwgbaeooi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gqpbjbgkc.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gahdwtkhz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gtdtgfjxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gdxhhoril.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxsvrzcsu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gpeizocja.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gawxyqodg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gpjbrskqb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gltneijxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gszycrmhl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gwbxecgpi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gntyjhgzu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gjhwdmesn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gshlnemqf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gwaboccto.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gulobdhjf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/grqopuaqe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gtdprcnfo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/grotuniuc.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsnusmtgy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gptahipau.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtmqsjmrl.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gxdovnidh.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ganblmilu.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gdxpksgjf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gcttkkmvb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gazbyjsso.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gdrnuapfw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnesygdtt.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/glikdjwzl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfhtycwz.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gozfxwxfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/grejntusi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gghqghprr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gezkzrzcu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gdtwmwmjq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gjmrxqmpj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ghyispqos.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gxjahwaqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gduwjdwnr.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gfmgdosvt.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gebcvibvm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gotglofcl.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gddqriuxi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gmjtijryp.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gonwsaptj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gfogvqpiz.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gkevmlixn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gyxdrggzn.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gosvtbkqd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gencgmttm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnidurosb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmlhswhxr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grtoffwed.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ghgcnlvtm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gvyigkffi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gpyxixpcn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/grxsvzcgc.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gzqgoxfrl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gsefjbdpb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glzhgphbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gmfrgfknx.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gcezshtxi.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gltozipbu.sHtML


<!-- 参考信息 -->