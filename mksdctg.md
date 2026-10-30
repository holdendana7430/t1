代发 wailian999

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gbecvhtte.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehcrcop.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajuqyros.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxcjrfkt.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gluwtmjij.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggizcaynq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlhusoh.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gsdncoktu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/glulqhvus.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gkurimejs.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnozrxfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gejhdmygr.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzakfzhje.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxcdwxgw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsgtyikmw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwghkhazf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmczbgu.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevvtkjso.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/goxfghuhx.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcmhlvii.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxjayuxn.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqmsvxu.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlddlfnc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gngaxpuut.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gobzzdlaz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcyqztam.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gntqjufow.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/guvxqjvrh.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeglnqcu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpfzvfji.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgvssbt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnaxysr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsdrqhcm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvyxiaoi.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gmntmomlg.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gnioxbqsc.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/grbwepqku.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/ghxpdwdqb.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gnzyqehid.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/grafizmkd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwshmeq.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geniwiijl.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnamaejrd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrrmodws.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtpcvla.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/grrkcsvtz.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gicydtfot.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuplbzkf.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfsgepmw.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gfpeavvif.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkczqrjp.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzsfoplj.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gythoimop.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gamwxpryk.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gogrqngmk.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlbpnjbn.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gwqsvupxv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/ggfwhdldm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gvyqzxfwc.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gvzefnfko.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadkarvxt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepaznsnu.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gztymngtd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbjvljl.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gtfmpvwen.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliopkqis.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/glsiljrgj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhgfhbml.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gikuwladq.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gitudmqim.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gbhnajvpi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfgrbft.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxymvear.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gxwznsawc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gveylnrtf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvdmvdamg.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevosembw.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/grffwpref.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwgvwpkpi.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/grecizplc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgostlql.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdvlxbba.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gutrpyhjs.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gccyanbtk.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdcfpnidz.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gdiabisit.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvfimtpz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvegsmfpp.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gsdlsmowq.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlnidqdx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxidjbaf.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgdshit.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gpufheotu.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gixbbgahm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjegruz.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gvtwgoyxf.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gwngysrau.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbalnwog.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gaqdsdlpj.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gpdbfuxjl.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/glffjjflv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdwvgdjd.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqecddqz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwyhunve.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkgczudbm.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gewecwxeb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptmbdrc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/glugyimuj.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvkbhqj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gkpuocxvr.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gklflkpej.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/ghhesquuu.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/ghzkepezj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjszsuf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcyytwxk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsifvzmv.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupldxfa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdywkwxgq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grjdpaced.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqwntzbv.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaddyidda.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtvadbse.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpecrvcs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpddqdzg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gpdhmdzsi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbzwcchm.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrsztttw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gielcscti.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkeobdot.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gumgvqngj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkzksrseh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gvzsywvlg.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/grbygoxik.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfllpukd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrghhonw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gbvuqpfsu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmehezlyb.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygezofoy.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzmlnwaj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gmrkogses.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gtrhfriuc.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwkccyap.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvxozazk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gsaokuydp.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduchklox.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gewkuutgv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkftysot.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gcecziala.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/glvtsjrzd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/glsewhamg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqjkhrkv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchkufnvk.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcommfey.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gglewkoqf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gljfdlfas.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gbltwmrgw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuertzdz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gyshijsxb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gstqvlfja.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gqrzoeaxb.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/grhyqhgnd.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqjmzcgx.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gofeeyjek.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gicodalke.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpsyxzar.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszmfcbio.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gltkplhir.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnadwjgfo.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gvqeholaa.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gwcvldtms.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyepocmkk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemiisctl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdnftrda.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnrsnrer.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genteyyqd.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gineoxkgp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbcrsotu.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gohomswbw.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghdlgyjqq.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvouxtje.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gpgrbknja.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gdpbslzoy.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gupcriybf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldnvrep.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gzmjyaeqe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gjuvehodg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcuzohew.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazuyomiz.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyoleth.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdkfalmk.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjsbukqq.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gtopoeqag.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/guuefrrck.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmiifuc.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gjmziubkc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gilpcvyvq.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywhlfvoa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwscjdyi.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gttlchksh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnakfawja.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqjymmtl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvddctwkm.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxqvjuv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmlsoami.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxqjqnbs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezakibmb.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfhuznlz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gtxnoczbe.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsvllmz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gwovqmrpc.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnhnjvvy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsvmzymr.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbytibfi.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gbxxlceaf.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpflsgeg.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gxlvjwubq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyvamoaw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubfrrxru.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/geffwhaij.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppwwgukc.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeiismxb.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfhkqijs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrbahrwx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqejvbazv.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gscbaldpe.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gspcjfihl.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/guwyfstls.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gysjvgybm.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gmsjfdbxd.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/giewmusdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/grfgrfzkk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabtnsnpx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyndmqbfj.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlcbidun.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkunpwabl.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxdjpik.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gffndwfiw.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkihmbl.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocspiwzq.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtjqhjty.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmojqoweu.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gysuxagmt.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gynrqdrxq.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gsbypogyw.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvbfnjjh.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gbbylehrj.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgwtxtpa.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gxfaoxlxb.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlpjzzpf.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gofiagvyz.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxzpdoks.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjancdmg.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiqjcreh.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqpgimex.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gcekesaav.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gaanetxou.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/guuhvjcfc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyahovbi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ghksgkuwx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gffbjzigx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoujrgda.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gobfrzbgw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbmlcglb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdcxcfly.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gppadnbmk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gfueigiah.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwiarlhev.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gawuwnaeb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grnzsifbj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/grreogyan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqtxmmm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnmxxpqo.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/glzejreta.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypcxveg.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/grzwuuvjx.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyvpjllr.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gajrcrdsg.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gogwyvpjk.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/giphctfja.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkgmvjpqk.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/grssvnyeq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmtrnot.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gggsdmnnp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcmicxqv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gsbjhtvcj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gychaxfhb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gscxrmnpx.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/ggefwuszb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gonzatdkn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gumehcbzz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/glknachis.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxktdphyn.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gtacfwdta.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gvrqmqmzl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxdeqaj.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gdtohfgxo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlahykqc.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnegbuzuq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmpkglak.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/guagtfobv.sHtML


<!-- 参考信息 -->