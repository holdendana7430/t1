代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gowjyqiqq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gdeksxoqy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gizjmembu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpnkmrzwr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/geywiegca.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/ghwjiuurb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gkxrsnfsk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gnngecioo.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gwrhvagbj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gzsrgbvyl.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqgjmluyk.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gwstkgtmi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gmsxqzvoq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/guzwlhplb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/glbetpyre.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gpsurxwbb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gtfuxeeqf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gvjiqprwf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gcoivcsqg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gfyfgnpyb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gwpniijmf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gfmwwrret.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gzptlvgci.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gjivbqmms.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gocgzxwgw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gxdmrhtst.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gotmsusqi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gtpssfybb.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gmlbjkyps.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gsrphgcit.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gusdpixnw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/glrneyweh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gxgqotcfj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/ghtaejtpy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxkxhmzzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gclwttazx.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gzwxottaf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggiqrnvkv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gayadvtwl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gkascxvhq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gkiknfcny.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gzfrhpphu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gzgupuboq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gqmacsybh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gqkcqrefr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/grktnlqzt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/ggrydhmam.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gzobmyrdo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gnizuprqp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gcdywsfhf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghhagsdbv.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/guhgnxuit.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gomqdspaq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/glxcmunwz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gaquegdjt.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gpheftdug.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gkphtmlhg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/givupffoz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gsagpkqdm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gfpdxzdfl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzvkjkmqu.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gpomibwxd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/giugghwlo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gjdenjavs.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/goovhvqee.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gybecvzbq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gfldyhoiu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gzzbtunso.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gmfsksxwv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gwgcynviz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gvuxsgbul.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gyyzeosnn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gqibqtkfz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gktyumgpu.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/ginxcssgw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gxwfhzcfu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gmmfzyzzo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/goyeivehw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gxuryyjac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/ggdvajytv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gdmagrhmy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/guophkkjz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gmyhfktsa.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/ghgcduycd.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjmzurthe.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gsocbosel.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gocmbefba.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/goxxcttcn.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gbhgzayki.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ghiblmupl.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/geyzzbmcd.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/glcehcofb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/grwhnqryy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gsfgxtuqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpsszczmb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gzrvrxbjx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gygclkvgw.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grlnmmvyp.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gclxevbko.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gcpntxgyy.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gksompofs.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gynlxpbtw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/grcgzlkpm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gjdfmmerz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/giutzwngk.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gmlgpqmxz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gacvtpkdf.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/goubuwerf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glpywjacu.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gkiruinyw.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gycqiadtz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqisbpjxx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gdchxykzd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gqqdvqkie.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gzifafngo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gtasydyvs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gufpwaysk.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gthegtjmg.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gdfedchcy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/grqclxlvo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gzziiomxn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbpfsalij.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gikjghgcw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gugoaejsf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gjpazpaai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gynuxwilt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gajqdkxgx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/glvzranmg.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gmqmngjyc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/giwqaqesq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gzvtyinsl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gwoebarid.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/grcquyfoz.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gsvtbmslo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkxzbrobv.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gjgziyhei.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gceplfweb.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gwdghfmfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gjaqwrjgz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtmzlrvpt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gsixzvfmz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gifwjndoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gtpbtcrgq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gacqjaqwe.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gafszppsg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gohidlshy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gejihwyxn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gkpelonqt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkkzsefgn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/giabnnjyn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzvymtipi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gxoecvivl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gxczijcho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gbozmurku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gqfsgvpoc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gmztnksjj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqgfmvdim.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gkfveztey.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gglrcfdel.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gbyslndqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gptxjlbjm.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gwbwunggb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gowkiwegu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gylugttfz.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gpqmsguwo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gquhbgrto.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gvvratvyz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/giebgkvki.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ghndgnmzi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gdtdfkldn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gwredmhnz.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gsvsgssco.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gcekodcby.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gqblqjmva.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/glvpvduvl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gaenoicjz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gcrvzwdmu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gpxactdie.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gefdvcdwo.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gyhtdskgz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gdmgmkqiz.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/guohbaipr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gwqyyqbvt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnnouhqmi.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvssqsakl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gjyhwuemb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gjsyztsrf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gwbbxsqwb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfnpyexkq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gbpjybbhm.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/goxiesbhy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gvrzqnrbb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gkdvpqcbv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gkchqherp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gybytkoqv.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/giwbszgwn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gmbtrppxb.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gvijieywa.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gyxoekqdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggubjjjww.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gtgvclzhz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwnnanuki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gtgccufpf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gburhpokk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gwofzavvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gkdczytdp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/ghohqzvvn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gwydaddqk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gwtdfqnns.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gopvxcxch.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gdpxqpiek.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/ggsbiqnnp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gzuzhodno.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gfacyzqaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gpqgsqcnj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gcqmwplhn.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gtpmyucmb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gdrafbrjq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/ggzupsbbe.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gjjwbaxyn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfjogwfrm.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gljdzbyzd.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gtphnpitg.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gmqjjcqks.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqcapebdp.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/ghqzaibit.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gubbkwjws.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gnmcfilif.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gwrmjxxlj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gvavunxzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gtedetlop.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/ghbtkfucf.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/glolwatuk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gsospvzbi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/ggsmwsfgb.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gsvmoknxv.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gmtryzbss.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gqkmlbygu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gznvjospf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gbbenjtvs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gdzagalbv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gamynutou.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gvzaawvkl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gydsbkvms.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gpampftkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gaezqidbz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gqolejtsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gmmeplddh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gapdzbihs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ggmhvmchf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gijdfeswt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gzmgshalg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/glxbbsbru.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/grkujllnp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gkldklyid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gcbcjvywj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gvffnumye.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gavucratn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/ghnndglqd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjftwdymw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/galjbqfvi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/grjttmztk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gwrusdqqm.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gjmhmlbpg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gqioiygim.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdjbupjzf.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gngokeswn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gipfyhwoy.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvcitdmvp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gkxnphfmj.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdiolnwzp.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gijgxmpqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnzhwwgdt.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gbxtlauxf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqyyqhupg.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjrhpgsuh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gghfoaiza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gzcexvhus.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gsvkjfoqw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpmjwmopk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gbnljjbig.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkqaknpat.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/giitzqpsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfcpeszws.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gxpewvezk.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gjyrqepfz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gzjxfhxrz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvicdtvus.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gaoqbdcnr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gpcpeftib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gdnojzhjc.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gridyihmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gcbzmpcyy.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/grggxehbm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/geazfbgim.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfswrdixk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkavwtlng.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gxipfabms.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gkqunbdyb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gnxtudlce.sHtML


<!-- 参考信息 -->