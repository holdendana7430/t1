代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsryusgye.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gkrdarejn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/glypncnxb.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdlioncvv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gndpuqixo.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gjlaaoizi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gixsmxfgm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gkwthtgcv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gegbsncss.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/glsudliko.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gghuixaim.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gfprjshkf.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gfvsjndhc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gmglhitlf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gpgeebybb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/getahplqd.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gqrozwpba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gbjqrntwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gnvlwvbkh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gqeirsbzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gmlmcgtpj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gzlceicaf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gotobehcq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gicolowym.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gglciwazh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzsygffyw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gmawtztpu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gqygfmxiy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/ghlnwfgyn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gxftudbvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gjpajzazc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gavbzzmnw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gubmkvooo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gouzeqico.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gncfuipep.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gwvpvylam.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gdnwodnja.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/giuwlfdyt.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtdsmrsby.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gbfyqrnuk.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/grulzrlhn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gfxkamybw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gwwbiqoxt.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gnuecqeus.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gdauutrjn.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/ggxlsgcdy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gpsebqsxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gjwgwzwde.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gspwoyadm.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmmshmgzm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gonlibmia.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gwqscxbol.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gaqcznand.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gefbrwwxz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ghttotqjd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gxefaswge.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gyimshwgk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gaxyaknyk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gnbeayjvl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/glmdrduco.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gwaifmqdn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gmwmzwucn.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/ggaiidhkx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gipeatrmx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvrvagqbu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gsenrgngr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/ggpzaifyr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gbcaevhkl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsbkdwvhi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gkhtpsdwr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/goseuwjhs.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gjwhdeeqs.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnocjpqcd.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gnhcgquzq.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gkiblqpbt.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gqnkpohyc.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gwlkwidol.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gwhybnhpg.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gbsdyzxzu.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gjlbiqhlq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gwhigpbwu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/galbsfdvi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdqwbesqr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqpyazjka.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdkxjnadl.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/glpagfupd.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gvimuzjkt.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gmfyaqcgm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gwukjtiul.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gsebxxddd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gwgrkybiy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gwzqipygd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gkragrghs.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gudvxjgdj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gohnpvvta.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/glgkwrzlq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gxhvnstgv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdwswbvis.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gmzkchrlm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gvrklhrpx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhksjsiw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/ghskgqnwq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gnkbihibc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gvjrlhlxb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/guaurvvxf.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gzhtbkzqc.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gvlszckch.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gfkxttids.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gsjyqavtx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggbwmxwnr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/galgtbczf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gfsmesgkz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gfjoayssv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gpdenjdbp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/glmfkdwxw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/geuzqwaqg.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gydtijbxk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkdtcqex.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gkfrvfsgj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gekgqfbal.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gyowwruyk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gbahbcbaf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gberuqhre.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gyyrnpcok.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/ghntcelew.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gtjumqblt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gupgpyman.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gaxvbnaag.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/glepkxdkb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjzbalqva.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gpehbibnd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/giiexdxwq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gncapamxv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gtldblaeb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gxvoxuhht.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/garatbzjw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gxawyfhrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdjsatigq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gltbwyhgp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gmmzmzaow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gkhacjzin.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/ghupmxkjh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/ghcsjlyfw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gnjfpgozt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdneqwxop.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gfdahtnnh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/glgiczzrc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gdreetodc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gnffkkqih.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gakjcvnqt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gldgaquua.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gmlibnnaf.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gdtjsgiyg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/glonarkop.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/guvvskxop.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlqozmx.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gtfjdjsnr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/grvugawhi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gaxtecfql.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gihfxujsg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggohgzhlp.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/glklfkvbz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxsvnadze.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghcsofidw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gacrkrmlc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjcmwjqfr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/grwjxsnmt.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gffjpbmsx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gojzqudrd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gotzqdjhy.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gwymwfygg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gwaeymdzf.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gvrmuqwpj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gfwiwbidq.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gkdoakkws.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gcofftutj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvsgfcmda.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gccocxdqm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gpsixugfq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghzewgnwm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/ganolcsmc.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gtjhzdptu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/grilgslzl.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gjspzpoxs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gqjjjprcv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gkiawpohc.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gvkzfxkik.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/grolfbhfn.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gvfvqztkd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gaxoeiuaa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gyugazlkt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gkuxuvpfv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gqtaoicuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gssuccebv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gvakrgyes.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gqhbuzzkp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gbjfvftib.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gvgxfesht.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gasjkimde.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/guykhfdsr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grgjafszn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkiblyriq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gikdcbfgz.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gvppwnnkv.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gpzmusyyy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gvojgnavv.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gsccxyntg.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gltowqcqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkwleamhi.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gpqjsijct.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gyclgmofo.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gyibrwebq.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsujwmlfh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gueokzety.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gpjpknnqm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gunzbifpo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gjumyptej.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzevdiudf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/giemrcusv.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gloxjkqte.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gsbmkxbyv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gsgznjfds.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/ghjqykwhd.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gqhuwfdnt.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/guriwujxu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvdapjwwf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gowtrhqnz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzijzrygn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gdfnqyjop.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gjtlicqpa.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gqbyorhsh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gddzjlzye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gskkummht.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/ggfafgcdx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gulcawfcw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gttvdootp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gzvnuubup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbadnlhim.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/glbwgnvki.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gqlsteckf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gjbtvbpcu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/ghbycuhew.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gerqcurvs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gnhjiujho.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/ghxsbajfs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/geqkdvgir.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gvzkmfsju.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gexkrabvb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gatrnxwpk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/glyfqafvb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzijbwnws.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gmhthilec.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gytavkkkw.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gcladkzpo.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvbwhwhde.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ggpskmfbt.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gitlhlwdw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjnjumw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gvkzqvzbg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gpuvukicd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfuqffnqz.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnriywpfg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsksnorzt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxunuceho.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gsitdfijf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gwezxtmid.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gmxsdiotf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gogcqseuf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gwalsduvs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/ggdskjrzk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/glypmzdtb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwumeksxv.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gbrxubagi.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gzuxaiafd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmnglktr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxmphtazj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gzpflmmfp.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gedxegpdq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxlpmakyq.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkikhctcj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gfrzaciup.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gzaoayavu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gkkhuqzua.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grzgbullf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gmhdteqzn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ggkviiwqh.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdsoprvic.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gqrvwulvk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gktqgaice.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/geqnzslud.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/ginswsqih.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gpbxsijum.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gwhhywlwk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gpmribgay.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gppowhuky.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gwzjrtjtw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gxeedxomz.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gxbcmdfez.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gjblbxikn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gllluwyzi.sHtML


<!-- 参考信息 -->