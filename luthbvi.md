代发 wailian999

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gfcccikbg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gyhnxynqf.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gtutznxpf.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gidoqsuji.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gbvnejttz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/giyvwsztk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/graecyylj.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gxyuikgtp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/greodipmn.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gryqgqurf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/grfnetrbs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gseoqowgu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvqqzttge.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gwvkxyqoz.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gadeaonyj.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gsasenleu.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gbssegrsc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gjlxfyiyq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gldhbxalh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gsemqkcny.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gtyzdbkkv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gmneasnko.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/guknebess.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gmwrfftrk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gjoecwykz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/glyrnwsdh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gkzsfzlra.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gozeritgd.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/grtcmqzkz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmhefgiat.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gyvsumnti.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/ggfhauliy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gxmcvjoud.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/grxojwoia.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gsiflrfni.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gxowgefyi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gcvyddbkl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gosnlhvhh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gzrdlwjdz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/grukrxijt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gtviyizyg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gbcwydcdb.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gmbxvnlyg.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gzziezbzk.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gddnjqvid.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gybylggbb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gomkkqkse.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gspcovhkb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gczldcxcm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gqkeuaxny.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gakbbkiup.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gwwpxwxop.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwhwdourj.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gyiircvaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gbvbqmfxa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gooqakzhh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gcxhkengj.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gizecadpc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gownitdas.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gkxswdvvv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtctmvj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/grelvkwxb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/ggffxyyha.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gnneccmxx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gwrbevzjb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gjjpbcljr.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gdqgbtvrf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbnwwmmby.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gadkyopei.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvhxcftkv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/ghtstoccw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gyetjrmww.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwryugdzw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbreptyip.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gyzyrwndz.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gmlnuryuy.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gimxduhgk.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gjboogdoo.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqjqoffrw.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwrhmifce.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/graqnonte.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtsbtegfy.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gtrrabsyt.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gtrjrqgrk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/geembfqyg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gratomzmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gpjjndsoe.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/grvlfcznx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnkekyceb.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/githrchsz.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gjuaamnte.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/grxeomsjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gofzmstai.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gcannufsb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/goxnmtxyt.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gnbfrehrp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/geyflotbq.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gesdyfoou.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gziohzkwr.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gffqfxuih.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gwxncgmsz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwqgoboml.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gcbluflrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gvbdwlgva.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggezewueg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gobovkrdx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gfzuxrzpz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gosngiqga.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gamgrsnli.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gbhmrlpes.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gijoskjtc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gbusybdxd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gzqpwmfgp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gaueqkbvb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gopyhexfp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gmedipbbb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gbwohuuvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gmgblnipq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gtiyukwjy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gykifyhdx.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gqofgtuvl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/ggztyvcoq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gbekpmszy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gihggygte.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gjkmnsgad.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gzvjemdfp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gcilpxizj.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ghwntjiry.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gbporzppt.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gztchilsf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/glxzrvsqp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpuiywlxw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gegrogmlr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gajlkdmik.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gijyqhaqb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxcxnvo.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gaxxnkobo.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gqucxypza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gjhexfvng.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gepfltesf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gmazbrhkd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/guxestbrz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gwconezgs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gryqpezks.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gkvmpqmsl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gihkjcpmu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqgicgnqs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gdwnjdnay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ggviblqdo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gxkoxhugv.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/godyvokwy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gnrltcuze.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gowdqhrcp.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gxueznzaw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gujstvnhc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtdqotpnw.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqcbltwqq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/glvedesas.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdrorehiz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gzkbtwbfx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdgxkcbre.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gpgkxksxy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gfcnwxqhu.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gtlmyqxkk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gxlfwqnvl.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gyjjdmapa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gmrxualpa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gyweeazru.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gqzxftcyj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gtaucfbaj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gafwzvgof.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/ggrxgyooz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gscwfjbie.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gkwaxpzja.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gzzhrfwue.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/ghthuoopo.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gspdvhqmo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/goofcrddj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/grmyajdfa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gmhlmhyyq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gekfsvbzi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gsmlpgmiz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gxkhfvcqe.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gzqpxinxw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gshcuwykg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gphgjpmbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gzlzwivaa.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gskaajbxx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmnxxkkbb.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gcrjvedkr.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gafgxooui.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbrhgszze.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/glhbtncmu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/giskpvpyq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gxbrigrzb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gxwyrkowf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gdtmpcwsf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gjrjasaek.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gggofjvgv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/ghwtbbhsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gyfmsovfp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gzzflchlb.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gfdeqaozl.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpjkhnmpm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gslovnsup.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxxxyhkaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gjelehcjc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/ghauzbqqm.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gxrcsairv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/giiufrmxs.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gcxhgquek.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/ggwccpjhs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gyzdvibwf.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gaujptlzx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gohobpxju.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/grvzthdql.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/givofyhks.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcynxiyzs.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gwcsqbfuv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gocdtvzwe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gymugqqsp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/ggxkvpyzo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gussgqkqi.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/girmcnrvg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gacimyclz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gyjiexhxj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/grhopkrkh.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gnstczjii.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gksqtyzeg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbxbfozfy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gxllvphca.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gshhlahrq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvpviqopn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gquvcuujq.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfyhwntwv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gxkwmxnzc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/ganyqanic.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/guyjasvos.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gvhihalvn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/glbinrktq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggaledvpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpopgkl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gjnryjfmz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/ghkqkfubm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gqrourilm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gqugkefkg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gqtkzplkq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gfemklqxp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gthdydqkg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gqormngba.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gmnqznsda.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gzwmzveem.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gldujlcsx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gmynigfkd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gxfcfjtdf.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/giqkzhrhf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gisfwreyz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghtptqryv.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gtsvrmzql.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtbfljfdx.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ghadtppok.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gfvuksfzm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/getxpputw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gsezlqzof.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glyvhmclz.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gwbhkisqs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfzfcovid.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gywqisgpm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gujbuchxt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gpfedstse.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxuxyjcxn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/glfllrceo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/ggszgbnfh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gjagxhdjj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/ghmshozwy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ginapxcxb.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gpidmngxv.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gjnrjjryk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gmbovrddm.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gceeamcpe.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gvlicyxuo.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glwxpvftx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/giniuvywm.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtccfqdqp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gqlwjeule.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gzvuvxoyc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gemjlerbq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gbkcnfajg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ggzfqybyt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gjdzsiirp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gfdxsrwfc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gcjukwfjh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gbtssmulp.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gqokzronm.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gtmouuoyi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gilgnsxyn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/goahicnud.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gcljvjdci.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gsnxnzciy.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gjongqkeo.sHtML


<!-- 参考信息 -->