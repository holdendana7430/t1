代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/govkybqeb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gcezdujmk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/grqlauuqc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grrheswwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ghnpllqwh.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/ggprmijgf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gleaafflj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gwrdtkxyx.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gdljapvdb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/ggvntlmhq.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/glyuvsjrl.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gbvpnncmr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxiqrufbb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/glayzrhqj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gkokkichr.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gfyyieuho.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gsmiabzii.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gyqmzmkpr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/ghxnxwnov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gevyibquh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gloqlrcxq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gtboplyvk.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gcgagaljv.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gidvsvfvq.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gronoxvgr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gqnxraser.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gfodkpdhx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gezfontwk.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gilcapdgw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gwduadyfu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/geozsaoit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gfgirsvlu.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/ghmbwvjpy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/geofixrdu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gmzfktnkb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gblqbzwim.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gbnuvrerd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjwgxuhmg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gozdfnqxl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gixrndxgz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqlntxyef.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gwooeeviu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/ghdtterqk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gbwrbaxvz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gneoapyku.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/goscnlshh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gmgwlqlsf.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gcbfbgdhr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gznwptpwz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gtirioato.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gaeyoechs.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gbakkjvtm.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gqgpwyhkh.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gvevicijz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gphtgdsew.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gpuzctrym.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gqvcmahtn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/getnoyriz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gqhjcoolf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/grfielqtw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/guariotmi.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/goqrezaas.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gygoipssb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gygydbwoe.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/ggdngirpl.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gdwpqkxzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/grbzkwfup.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gburhkjjy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gcdbptvgi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gkhofdgnc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gahsjfamq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gmcjxsbat.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gemhpgyee.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkxeloqh.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gvxqouqan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gujwfgzui.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gqulvsvxu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwgdwxzpc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/guqipupxe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gfxprwxqf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gfyqvavjw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/glhgmwtgp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gknihmijk.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gxaoryfba.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gonxtdnsf.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggyemlqxf.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/goynrxffe.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gtclxihov.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gnbzacfzs.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gbhfjzfuk.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gqkktlhgj.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gxmogxnek.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gveoifvus.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gobxakklz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gttipwnln.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxazetulw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpzxscis.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gnuensloi.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gktxtjqwh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gdwhshfrz.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gpxsphset.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gjevnddcw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gltzqqshd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gstvoztxi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/giemkapar.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gguuipfzy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/glkzucfch.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/ghaksacho.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwazqhkte.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghjngtbbs.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/grppxsiac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gslfttrmh.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gzwfikquy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gcnuraxpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/ghiqjyrdu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gdxhyzkzd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gzeczsajr.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gtjawnnri.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gisyigxwq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ggwjipndx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gjykmjrgi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/garjdwxlv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gzalhedgx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/govgpwwyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gvfaovqwr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gefnilucz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gnikmxhhc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gfkynafoq.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gpwabaqny.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gbtuzgxws.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/grnedmbro.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gvgdkwnqx.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gcrthbeqh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gtgzkawpq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gxuiwimuu.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gydecxwqq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gtfyhlwxh.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/glgkydljr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gxvxyhgxc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gtvcdqhpm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gaojfezvf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gskdlnlbp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/ghykwdoxa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjovgfous.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gjziopbzh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gixshnblj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gstoxzzmq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/grpezgqse.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/geeokzdad.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gppnntgls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gaezfusdr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gricybzus.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gwgozilgg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gwexpqejx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmddgspbu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gfasrxdql.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gnrhqaovi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/ggoguhzls.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gmlmpnyxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gyepjqivi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gvhpttfbb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggddiyozh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gzrpwoecg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gjztghxvo.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/ggibyuwyn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gfuszvbcc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcnncunil.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ghqxsidym.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/grrhpourw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpojatdqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gjhwfbkzy.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gjvmebktx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gdtuvlraf.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gcfgkybpd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gywhnvwqc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gxnseuitc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghlesaznh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ggbcbsfjj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gpcqphlzq.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gkqpddvul.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gqjekmfrg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/glfrnnlyx.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/grnxsaran.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gzyantupw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gsepigifr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gzlllqvww.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/ghtpavhwq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/ggkqyjjss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjskoucat.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ggfjfaigp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gqionvonr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gamwyktyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gxvxhqouy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gpxvnyesd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/glbnggsvg.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gxmjkbvrt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gtjflddvv.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gnhhacwbl.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gvfasbjng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqpuggwck.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gfmphxpyy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gemsayxpm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gygekwuzo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gzmtszwgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gchrsnfxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/giyahtyxw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gbngmzamx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gifhfaisu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/guxwzgfwx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gtvpjtlng.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gtunxlidc.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gimwwlvyy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gzoqezkue.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gotkkxxae.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gtdaifahe.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gxmmejzyl.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gwtrltaoy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ghmuummjh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gxtyktgyg.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gasyjuagt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gcrcvegue.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gmnumxput.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/grymsgwyk.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grogyyiyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/garoppocj.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gljhzirzw.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gpbthpcmh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gppwxsuua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gvafrguqr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gpfcjfjcw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbgqvxmbs.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gurvporri.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gedhqktmx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gbqppetlp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gmlbihzsb.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/ghggafawo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/ghebzznkc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gzkmbcuua.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/glpinorly.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gcjtuzjbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmlozwnmu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gezxozzhf.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ggfhvlmdg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gopikkngj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gctrttfem.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gflhdajpp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gydbtfoal.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gyejwpljh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gayqnwewi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gubaufyzf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gqfekpddw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gsvmmmnyu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gpaiwcvof.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gexnrsagp.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gseqoiqoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gliscbwvp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/guwfdiitm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gcheztwlt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gqwugveif.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsalpgeyf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gyibjiolg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/grefpwmcx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gybizatgn.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghuxphrfz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqfzcugpk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/guxorsshh.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gjaxaxyoc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfnqpudje.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gzngzpody.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gsqkqjjcs.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghnfganvd.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gptwklxxh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grkbexrej.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gzggqlwua.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmealrvrt.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gpubunams.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gtfykwuni.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjevppdz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gmfqttqvb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gmyqjcrmp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gndxagmog.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gyvrlbwig.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqjvqawgk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gishqfplf.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/glsawfrgc.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/grylhilzh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gziqhwbfu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glquozhlp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ggwjujvtt.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/grxnpfwaq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gxxngqmlu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gpstkxgkb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gauupreog.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gicrdcigs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/goxprccie.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxmxojtmz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gospbdepf.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gktwjeyry.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghgkjnecw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gvttdwuqh.sHtML


<!-- 参考信息 -->