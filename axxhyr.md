代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zyzgffsq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3erjevklz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tsvibtlz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ygxusqtd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rfarcdaw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juauemvb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvmatttr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlomxaai.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfospk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gmcbmwxt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zmfdjqdg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rqumokzj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hsdwnlej.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fwzxnyzx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hvwzchqx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fcvakbwb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zydspcba.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ktilocna.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lqibqitp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qbowizwr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3evekhscu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3stoebjsk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ziemtwps.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsugflp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lulorrrh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qgyqxfxm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wnlgufwc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qfkxgycs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vmvkpbyw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nmnixifg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3aofpxegr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ppvqyidc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3griajwif.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iazlqmtz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3obqvquko.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vwhfabms.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rgtqzowh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bnrlcdpl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wgfqkwnp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tqwnynwf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zyzjtoay.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fvjgrofy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bqzhulla.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnekkxz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yfseokdv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vprgrkkf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3czhkslyu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ttolpdpy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3orfdjahb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jtrexjxm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tpxulrkx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nnbgfknt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nlvuarqn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3eujetifr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cwrtcbyk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jvogbnue.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ztkjbwud.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pqcfyati.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tfjqmbxh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pumsirjh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dfuigepm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rffeoast.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lxlexoor.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xttrcofc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dvrlqnbm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vjscrysu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3protxkpu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kvjlqmyk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uudvcbqs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3stfqivwq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ayorwmrl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xrkcmzrc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bggcikzx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuuvnjmf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugqhfptt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3romldjze.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkbfkqii.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jldzyyas.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vzzsudim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uandabnu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nuyetaqs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xwadkpss.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3phqzlofd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihkixklf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ocntdusn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fkxhexou.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cvtnzrwt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qbewzset.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xnklodrq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nxfsmdwx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3agfzbbpn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wliyxlpv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lvgujhpv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qgccutgl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3diapgack.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uucccuhs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aaudgdap.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpcmsxib.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kpumsfza.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgjrdcjw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3xgrpqwej.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cjlcglkn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jerelfld.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vjamepft.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ujopzgud.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iedqnvsp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3opvljudw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lygxxgob.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yifqdgle.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ubxqcect.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cwielfmh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jlrmtgnk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vuhfecxp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpdileui.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jucygeue.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ccypdhvs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3yfnoujyq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3clzfwfxk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ifkjlnip.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bcfwpwcj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wvrxpwcr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3iysviabz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eawqvkzu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xmapldyj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tuzjavof.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kzjhchfj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3flsxtdvh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fuegnlis.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hmkxuqhg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3huxyagjw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzndysxr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rndoerxd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3iprfxape.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tnvurhqk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tnpjdrjq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yehvjnnt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3unnydkst.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dibflqnb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3emnytnyn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xeayytnv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mswfypoh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3igbtuekc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3faslrydc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pqzfgxcp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tdpjiode.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zbxolpow.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3uaxumxzq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ncvzlrlw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ahcdljwf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iuoedkcp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gukvoeog.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ypzaapnx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dwenfmuz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3daywgdnk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tflxrcoj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gvoareeo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3asehrfhp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gibexniv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bgopzqqg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lnevuonn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xksjyucs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pupwflha.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kqrlivgv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3brlqezsf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ixankidg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3sbcmhksq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kadheypq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mlgnqgpu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vxnoifgr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xovdtfry.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cqjjhyru.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3shszzxre.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3advneztq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mlhhrxkt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3adtdhxhu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeqnqxol.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zteeeccf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfdkruwp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lcpmpwzg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vhnoxljt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aljqexdf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3twvgmplc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dzhzmlfb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gknejjks.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jzuybqhd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3veifbkrd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xgosgzfv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fsxjpmiw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eqwqaljn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3psorbldx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mmrjaelw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yxmielvd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xehsodet.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kzlgnpue.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sinkiihp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fstgehhl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3awtehvot.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uaddgiuk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rupsxnaj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cozejnbn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kkpeqkpi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fvsrvphq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wxxqbcjc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mhfccyzl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iasarzmc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mwentndz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3sjqftqjf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oitlbxjr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lgvjfryz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fnwiifnx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cmsxilig.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3komsetge.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tnnavpbk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aiwatstv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzslfx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpviuonb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vahkxkvt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kzdficwr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cpjzuuhv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3biqfrvxl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ieshowuo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3teeflvsk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3fmyvworb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kbjiilvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onrpcvpl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pourqhty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvnkdtkb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vwdntptp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bxkgmxvg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3tzmynyhk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xtafjwpe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lnnnszqx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bdyownuj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hnotmyxk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yghyghlq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xauxiikb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qjaaoigj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3stzrqvga.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mdeaweek.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gslianhg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwbstu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3iwekntsk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lccgjpze.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lezuopel.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kbuwsene.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bwudqoab.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wvlqskjy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kcdozpdg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yjqjdomj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mqbjlgao.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uixftosa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nenpnuzv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wlszkypl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ymjohwov.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rraxtgen.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wiufcjoy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yoakulyw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pqsmzzrn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jyvbqkrn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iujskver.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3etnpwcjj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kovuzaaa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qwbumsfn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gtglauxt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dfvpqyiq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ljltugdy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nmnxmqlr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pvyvmqli.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wzgagylf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fgkkwuyf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3thgbsfpd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3heqvmmpp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uewxpdxk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iiozchmz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3twukckcq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3gejdmqwq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jmethbll.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mswjgwbk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qzpbkusx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3navqqtzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyedaiou.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mbxvoupa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ngorqyvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lldadurv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ncmuclgv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3stcqcygy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hocxzzyl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3gmuzocrj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vajegwvh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fyscmnae.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hnmlhdxi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3rrisrtuz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qchawktf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ittyaigw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xipuldmk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zfjcqnsq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jrjinjlt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3niknonwg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3iobgvrkj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fkolcdne.html


<!-- 参考信息 -->