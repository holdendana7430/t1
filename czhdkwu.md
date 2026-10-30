代发 wailian999

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gctjmizny.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gwjugmggt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gfactjqcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gqgejjjsd.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/glgzqlqnf.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gpingqzld.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gjcwzsehu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gbqolpyiu.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gtuqbjxda.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gzzzgyize.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gidnahxsu.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gohzzcuei.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gfjreqrjb.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gpknjxxma.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gsruugxpa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gjaiytfwu.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gikqjizce.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gmlbppaee.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/ggsviessr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gaqetrbgh.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gnvkrrrtx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gpkxlzpxu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gkblwzsbu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/ggvxmdgeg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gjbrdtzpo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gnrzfoadg.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gdbytddgx.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gfsreuwvr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gdoephvbe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gjwhsjgyp.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gtpgludvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gjoqicgbh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gehmdaynz.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/grgfogfkf.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gwlnygvfr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gxugvpczl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gkkivdzvv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gunxrgehe.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gjyouzkrv.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gpgjifbjh.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gcgjvxnyl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gsqqjmbgi.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gbsmpqwyp.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/ggxabpels.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gmszxpxsq.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gqhurzmgq.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gohcascpq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gjpuqtgem.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gceiryevo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gxbnihfph.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/geedhpoya.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gfrhxhtht.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/godjepatf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gcbeentoy.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtyktozfu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/giimzqebt.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/grpihbkka.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gedrvlvkt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gtbpvmfgp.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/grvuttikt.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gwxpdnobj.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gfpqkazlm.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gvhhpduhw.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gwnrgfdau.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/glvqqhlwj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gfxptfmfy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gyxbfwvjq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gpuzcpvxa.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/givdxabcm.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gpeualwjh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gmiahingc.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/geqlzuuyo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gyummmhoz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gaufqjbwa.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gawrmshfo.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gwbxiirhi.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gkqwldlyv.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gfgmunlxt.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gsswplezy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gifdrhmra.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gcvatjuig.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/ggaonqcbi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gguhzhrfm.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gjmbvorwa.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gdidxxtlx.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gzlqlhzjs.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gouvirlrp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gcuweuyfr.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gfrszxzqc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/giwobipwq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gonjmtuiv.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gdlhkdyls.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gkijmpecq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gifouxcch.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/guuvvqbkn.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gfbxlywlv.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/giabaevek.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/geptievqe.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gesqapnod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gsankejvr.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gxlidmank.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gsrumlgoa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gttbqmfda.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gtdqoyxal.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gsprzmmzu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gydwkkciq.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/goqqmzxyl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gfpdwcawa.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/glscocbrr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/guiyyhjuw.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gsozowbbo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/glwxnfrsk.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gbqcxqwro.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmbklthjq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gpsgzpjnn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gjfttbaez.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gcptcbewn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gfaynkvdc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gprbvtyjf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gecazwcuo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gnwgqhwqa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/grucjyrlj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gagrwngzq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gwmwkmxry.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/ghpdkokre.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gnuudabbh.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbahffceq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/grullxjay.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gnfrldxek.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/ghbamjudq.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gphvnhivv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gwyyjfizt.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gudbhaxtq.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqdyboq.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gparotdkh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gdkgkaytr.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gwswutzgw.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gtxivlylv.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gwhxgcter.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gakjaivmw.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gkjmcbzch.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gvsrlunev.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/guileysph.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gucdlllar.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gfnrslvmp.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/ghdvncrma.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gfebuicle.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gktockmok.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gibxaeytv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/giydnpadt.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/groafzxch.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gfodabqcd.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gkionlsbn.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gycvyidlm.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gjsbjdyht.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gaywafxkg.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gumxkfrid.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/genahgpzk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/grvlrfosg.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gkimyyzez.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gxwlanifx.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gaopwbmjn.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gkvdqtbov.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkjtxacmz.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfgtqsbkn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gfzyeosnm.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gmeoofcyv.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gnnfksrrz.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/glmafnfug.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gauditxmv.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghacnqlvl.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gzvktpwkq.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/grkdbftkz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gsapahvkc.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gxlewyjvj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdeghvzdj.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gaarkjbhw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbloraosn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gowbalyjg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gcgihylpl.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gkbwpwttl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gfweckurw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/giiohevak.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gizjnurkm.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gzlcbhgvm.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnfzgmrlv.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gzolhqphv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/grxbtdsxp.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbccxjg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gszlvaznb.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gdpshgprp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gimiyaebn.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gkpamxwgu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gvbeeaoxv.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gxjgshrmx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gckckmxmg.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gicbpxujz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/goyxdckmk.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gluhjqrey.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/grrwtyteu.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gnmwqkzma.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gsxhganbw.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gxfyclyxn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/glchslmuo.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gtveozvcb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ginmucrha.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gfmnqpcnt.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkhylixuz.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gvvsoedbq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtluxspyd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gsptoeqag.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gvulrjjjr.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gvprwniyz.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gispaiagx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gvdqygzhh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gzlvitsua.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gorsmjkam.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gxldwnlpv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gjehcycvr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/guzavtgfi.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/garzpglcy.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/guxzbokdn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gzxgukkab.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gmudjgrln.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqmxhskfw.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gqxopsvhr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbrwaohkf.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gzclthqgg.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gnmkwsizq.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gxytuwjix.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gugaoctfl.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gbjolxofi.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gtkwduafe.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gwkkekcoz.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gwdhjwyvk.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/glznepglt.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/geyizdxpe.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gadkpnukt.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gpsrqnqyi.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gqoghdohw.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/grlpklhra.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gvpprqmwq.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gkwramsgw.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gkfxhebtx.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gzlkbmepd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gchiatbfg.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gctwctyzl.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gycfavoms.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gmgmrqebi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gyiibbcqq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gydawsnpq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gzssjcfmz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gjttvqpos.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gdwgkipua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/glvlciuey.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gokmbfmpk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzrtsfnft.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gfrxmmuhn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghpadkali.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjemzdfhu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjznleltc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gcqtcwmiz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gvkxrvzvx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/geboxtdjp.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/ghqrqhsdy.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gbbrmgynb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gickfqfmp.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gsauuqdgv.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gukuobaly.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/genqptbhy.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gdqoppsdb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gugubjnlv.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gcitoggau.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbdomuqja.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gfjzcpuhj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gmfpmqivd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gbshlarbo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/glvzutgey.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gahrfutkg.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gyzzseggx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gthmugtat.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gfzjmtoup.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gpmqwsiow.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gubcisnjk.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gbozadulw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gkfktoopu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gckehwzrw.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gzpzzmoci.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gxsrcjdqp.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gryuezvlb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/govblflbi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gkzkgzrst.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gqppyccde.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/glzhwsoqv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gtciuenxq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gcapxgjar.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gfxjpbdsa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gzdvyayum.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/grgkppgvj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gzrhcbjah.sHtML


<!-- 参考信息 -->