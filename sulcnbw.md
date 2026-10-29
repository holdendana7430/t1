代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gclusxrkq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gwwmqdcuu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gncbghhea.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gdwqvfkyj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gzglaecmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfqwkdkmi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/giwflfbmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gcmbsfbbr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gylrtslor.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gbavxijbm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gdxmandyv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gijljmtvg.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/ghtpmzasj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gletjadjb.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gvxdlikpl.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghjvhhmlq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gtpivcnxf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gctolsmvt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gmdfmzixu.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gngajlehp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gabrobpgh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gmfcbsyqb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gingqmkdo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gnshrjcnr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzmnivdeb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gylfblfxy.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gkpuehcdn.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gvyvhlcvb.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gtsguecel.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gnyyeemab.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gghijqgof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gfrsmzepi.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gwvfoytcm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gmqvbqzep.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/ghtzpmiaw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gvbxizquo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gmojdsdxo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gsaoxdbwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gasvlclsy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtrvjujwa.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gsnlpgkch.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gadkfglzl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gjqajgpss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gxmxdudgo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gsnxfbqfp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdakrqiwv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gslkjpmpb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gheewmsts.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvgbawiip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gzxrvbxqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gykaorrmi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gstrlxfxm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gdezumkiq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gvsimsxqp.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gywqcldhk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gqpswtlyh.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwibzgjww.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/geazbogsk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gjdrzzcho.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gemxnzrkl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gvivnmckw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gpwmyetfy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gxycammxw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gqvwxtmun.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gflvkzphe.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/giaetzdvv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gvgdicjjt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gljmnorqc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gnuwrfqpz.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gwdsnmnty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/giirzalqu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfnhujdar.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gmrjzxudb.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/giepmtnli.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gtbsiakae.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ghsvjvtlb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwlyddreu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gmjwixppn.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gfzdaribl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtlumazfg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjvcbyvpe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gcsjenswc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gtzuuyajz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gkzgqrqkk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gysbnnpsq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpqxbhwhz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/goeazwvie.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/googmgbln.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgttzvfa.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzacmoigz.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gbjpzgvlr.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwxmfbplp.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gohkjdwxi.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gyyhcaehw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/ghqsjjvhi.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gpsutengl.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/glczdnlxo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gguzkikzb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkkaouytd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsrzvzqjj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbfcxdgud.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmtvyxabb.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gwxiztojz.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gibisssrb.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqwdqzwwb.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gagfblxtw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gdqkyxgzh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gugktyizz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gylhhdmck.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gaxeclmdk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gunfiatsq.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gmivxpele.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gyozhesap.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcjoiuluh.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/ghraxkmjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvxzqjrka.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gjmkwviko.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gulfibtvl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gyahrgbwm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdqpcacmk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkuezauth.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ghvpexubh.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/glenwkdzt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gvrycilhn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/glptbywyf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gbnjreapr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ghdbotjgn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gwfxepkqt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gfdjxlzet.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/ggpmtpaxv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gdfuwbnkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gjpzzabkk.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gtstikxex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gsddsyzzo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/glonhqccb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gxqptjrav.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gqodwfyoo.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/glyjpdqaj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gmutdujjg.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gnnovxroa.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gdaalokkk.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/glwksyysn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gsfourkdz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/glytuasha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcftsyptv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyebsame.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gcrbkfaep.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gechayfaq.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gpszmclcw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/ghyozphzl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gyghqolwq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfhgyotqm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/ganmvbvtj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjgcdxwud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvodhuxbe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gctzhwrwu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gjqahlejk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/giurksfmv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gezqdnktl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/geulwmjil.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/ghwowszgh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gvpftsagu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gijgpvudy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gntezurjq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/goekapnez.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/glieohcps.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gjypbknfj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqzsuadpo.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gthveeayc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpqllyxel.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gdxtapaqv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/giwcxkqou.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyurzgkyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gtxdevbdq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gptpkxyww.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gdzujmqlx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gboesgiuy.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gtmcfhlzj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gunicbzox.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmmedmviw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvookenoj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/giobqvfcz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gxhkyymib.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gwgopbwgy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gedqusulk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gufotbgfc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/giqdkdyeu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gzblfbygm.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/ghqfbcabf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/glzlqqngy.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gqhijntdm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gyhrojxkz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gyhntpuap.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gyaqaakbo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gctmtbybc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gimbzgxfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gkrytnebf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gtmjlexqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gtubqtokg.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/grnxfoniu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdnifwuen.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/ggnzntwnc.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gahgyblwd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gootgcgqo.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/grbippwpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gglgrfljs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gtpjzouzy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gtxvptzsg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gkmgmwnhu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghoseaiqc.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gkktigpre.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/grgexxqlg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gpbqesekz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gluswhmea.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gebovckxq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gypkppmyn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpkaesmwj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gkwbwpsxj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gdolpxufp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gcmipyleb.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gtwismouf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gkbpjsqzy.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gcbfyqsxx.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/grypzwhvl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gkkosgvxs.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gywbfospp.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/ghqhegidd.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gbhbzlebc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gklpseptx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gptgmcwjl.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjxqlpqdr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gkapxmwbd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmwekkijh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gktulhcde.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gaxnybuhr.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gwwvgngbu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gcedmxsoc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gvlnavhij.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gqhplnpld.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gaxjjmqjk.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gycjjoefl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gkjuxbksb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gaovmejww.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gibclckho.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gasugtpza.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gcdohtxgv.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/grtsrapfu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/guxiissvc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gafrfoytc.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gszzvggch.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gsixwemti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gzdnjdark.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gkaeynllq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfohupzil.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/ggufhmdiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gxqkvcjrl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/geegmfcsz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gbrfnvvuc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gbpmzlaff.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gqtrnsgax.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/ghkpzailr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gzxfvvqik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gwnimecsj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gklnahbfe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gxtasogrb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gsdvwlrxn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gavwnilpi.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ggdzbvwwm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gprkkhnqc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gkfwtekpt.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gckbrpvlz.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkjjscrlj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/geaqjjcjm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gotgpcvvn.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gxreemdzb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gvucpdwfk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpobzlszv.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtzsyeend.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcwgmgibz.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghrabtuxb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gjzfjlvng.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gaouyskwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnxnylgnp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gnqkbkfia.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gvbzoiabr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/grrszvtfc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/ghajkvwwi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grlnxncby.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gbobbwrwr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcutrly.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/goishjlsk.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghcksgxsf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gdgxkqfhh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gteihinet.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gnjwjwjni.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gbvdffqan.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gcwmcarph.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gosezanms.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gebmxslez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggbobkphz.sHtML


<!-- 参考信息 -->