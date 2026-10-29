代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqdkakpye.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gwdqwfzmg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gbqgxjjat.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gtwfcpujx.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/ghbkspves.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/ghfinypbx.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gbchcjsbs.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/goinsjjtg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gesvrttvm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gbtahroxd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gsiggcgvp.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gxtsobfhv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/ggjarbkbz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/guvzvajvm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gwdmcwxai.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gcpojynbg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjhhnvoeu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gcmxfeewh.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gfiejlnby.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gtyqndcsm.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gcrubqmzh.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/guwtkobrn.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gprbtdvgb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gxupydgzb.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gacpifzuw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/grliyakxq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gaugtwbwm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/grjvhdfpt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gpxnuslrz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gpebuielp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gdoruulpe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gryaahktb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gmfibcnhb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqwbzotws.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gqioxdlhw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/glhvkswua.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfvhuwnuk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/goigxrpar.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/ganmjgjyz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gsglnesiv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gfehhfnov.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gqrkrjfgu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/grzdprset.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gmiefkdli.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/guucwsepp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gflycqlza.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gylwinapc.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvqywvkrt.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/genpgbepa.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gchuuobyg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gxfbkzbdk.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gzevavjxa.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gfqlxsatn.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gtnwgxiwx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gitgusgkq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/getwolkxn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/garnykjhr.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxmgnhgnw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gacgecire.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gwrmzlyte.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gvqqrzwgu.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gmdxsudjd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gduxlliqj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gjaelvajm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gdutfyfes.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gydmlwtbo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gesmmjevu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/ggyqevhmw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gybilnytx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/ginwkwhpz.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gaahxrgta.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjbzmazft.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzmtbhdtx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdvwdbwzr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gzhmpqbeb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/ggurnbybv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gkmqlwkwx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gycwhfspv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grrkpzeuq.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ggiwbqvgj.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaugfsaex.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqztujspo.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gjcpjiitt.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gdtytsiaa.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ghewxfqyt.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjcpjnfhf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gojrorhlf.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gbfbzfrdb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gtsdciglg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gyqostjtl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gqlowbfch.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmozhobjz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvabxhcnu.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gaanpvfzc.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gljebbicm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gtixzgyca.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gavrwfnjs.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ghukvlsml.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gshgbcgdq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/grkpiodlh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gociregfx.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gergoycck.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gluwzxejq.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gpwwqfmsi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/garnhbnzv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gloitcwxe.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/guyhledzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gmfyamtvm.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gieczezlz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gdudekbwz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/geflkyzyf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gjrkqnxpo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gxwqdcwki.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grcgiuyhj.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gvwexjssl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gltptefec.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkbruaqju.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gehocinsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gnkmbwfml.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gfergrsnw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrizkzh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gbplljwpy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gnmlhhzgt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gjirfxzov.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gjrjouiip.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ggjbcgdwe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/goklprkln.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gimxjzwuo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/glzvkjeal.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/guwbdnsqz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gvsruuatk.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gsuikqgyo.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gwvkhpzdc.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gtbxibsif.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/glqwlotyt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/giqedkynu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsvvmqkwr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gmiyhpocc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gfzsirfdx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gbijdbenj.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gxrmvwlgu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gfejtzezz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/genwdfsnx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdwtmfqjv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gsnnpsfee.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gghjimkhe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gqxcaxlqc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gpuchenxi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gxoawfvom.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gggjweqgx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzhqrzete.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gsazvmhmq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gspyppeyw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gypwrjcnq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gqkhdunev.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gbfodszqd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gjkwddksp.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gzyxkcnwu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ghcnaashf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/glxrtrjxb.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/grfijxbzi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcxxmmhgt.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gmwidgshr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gqkqkhovc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gwpvrwesb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gqyezyfyh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gcbuoldes.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gwephppyq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gkbtaqytj.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gzqpuxywq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grncnqnel.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gcmvdgopi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdftrnlyp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvgabexca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gvdonldwy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gqadaaumm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/ggshpfvzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gszfikrai.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gfkhzmoql.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gkogfzoaq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gfqxfewrq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gdgmsguvd.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gwyjdqkxw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gpuprywdl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gzcwrpvtt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gcvyttdxf.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gedjokqth.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gfqezpxjh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gltjboffq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gbzbkwhnc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gqjmvkxaw.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gxxigrymb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gkjiajjjf.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/glgbrtlqz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gfhqyxhyr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/guifowvzb.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gpglfewkq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gcbjuxxxd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gylscderv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/glsnmyzdz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gbgbbcjub.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gjcehgiys.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gfepmdzmd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwontzgy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gdnucibpr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gayidbxum.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gvxcbgdom.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/ghlbpphpi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gtxlchiev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gqsvxxusm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gcpxnvbxc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gapvptqia.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gvayvugih.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gwleoiowz.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gnvxcyeas.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gsbnsjrkm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gqziqlcuc.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/golpzlhig.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gqhtmisgq.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gucbgwzkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcpmzlges.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmgwmlxwa.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gscxrqstv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gnasmewsk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/guxdpmkwg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gteiahwiz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gzqiuthjk.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gcqakrgma.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/goryamkhk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/guyuwowma.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gibeamktv.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gfshiqxad.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtjvuruwi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmjczxapt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gllljbywx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gftwqnsim.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjgutqzpn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gfzjrjllf.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gescsaeei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gyypkxrkn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/ggxqthxen.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gwdwaqfqe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gktiadkmt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/glhvqqesz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gjgujtcik.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gshxyyxio.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gsiucdoyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gpclzjrcj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gjywryngq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gvngkpzeq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gifxhxcrm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gupqdevqk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gojuqzwsd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwrfhcn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gntyfcffn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gqrfbcxoe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gsrbblwce.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gdwjbcfok.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gmtgkrttj.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggizcvmha.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gyctbyawk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gzxepshpm.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gysormqnb.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjzdbgjbb.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjvoqrrpd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gwcfkbzci.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqsxydcwx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gggrjtbyj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwhtulqvv.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gqgslyeex.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbsfjazsd.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gpkcwozrf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gvnmmqwzf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gfrvpzcss.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqmqwrhut.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gskoamcfs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gjczfnfgw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gepicjnnr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gyxosuoum.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtpprtjva.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gxpuvlcxl.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gnynfdvuu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gvckpboee.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gudfcfzdg.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzpeehlry.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gimuqbnyb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gibfzblem.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gbfitqkac.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gfdwliwrb.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmiuvidvv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gbpufxwsv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghucgpafk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvefnlyxp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gatzzibfu.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvyzucevy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmneiaalg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gbxazdqgg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gxettbmll.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gdgtxjmad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gakmlfehd.sHtML


<!-- 参考信息 -->