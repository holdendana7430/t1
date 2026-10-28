代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hz.pycfn.com/gtopqezmmp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.vqdsnc.cn/gtfqtlyytu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yuanzhike.top/gtwtywzhjt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhongyouzk.top/gtdohzzoog.html

[U03] Py：加载 .env 配置
来源：http://hz.zycfv.cn/gtqffpmzvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.52xcode.cn/gtljrpvxfh.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gtxkbdywno.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtzwcrdahp.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtoxtcagok.html

list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtoorpxcdk.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gtdjtpmlos.html

{**a, **b}
来源：http://hz.yuxming.cn/gtljdroxxn.html

[U07] Py：反转字典键值
来源：http://hz.jlsjyb.cn/gtqydyxqxv.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtbsqrjhex.html

[U08] Py：展平二维列表
来源：http://hz.ehwqpu.com/gtvjmzwgrs.html

[y for x in nested for y in x]
来源：http://hz.yangfankeji.com/gtqdbsxcdp.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtrghfocya.html

max(d, key=d.get)
来源：http://hz.ppjwa.cn/gtgtamfict.html

[U10] Py：按值排序字典
来源：http://hz.zhixingplan.top/gtwykezqbs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shuidangran.top/gtepjvsshc.html

[U11] Py：生成器表达式
来源：http://hz.tianlin.xyz/gtcfkhdwqx.html

(x * 2 for x in arr)
来源：http://hz.chenlongwang.top/gtmncmmbof.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shzxlz.cn/gtoomjdsst.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gttkbhdqjp.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gteyhbgbxl.html

deque(maxlen=10)
来源：http://hz.hongshengwenyu.top/gtjzecaljj.html

[U14] Py：分组收集到列表
来源：http://hz.guannengcc.top/gtggebvmhm.html

defaultdict(list)
来源：http://hz.tanke756.top/gtwbzsjvbl.html

[U15] Py：高精度计时
来源：http://hz.gzhubu.top/gtqfppjjax.html

t = time.perf_counter()
来源：http://hz.sufxvd.cn/gtevjvlxqi.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gtcnfsxvkj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pycfn.com/gtqcdlftxq.html

[U17] Py：初始化日志
来源：http://hz.yueranfly.top/gtbbfqkfca.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.snrcjt.cn/gtmqspdusv.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtldszdqgl.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gtsjqewsap.html

[U19] Py：正则替换带回调
来源：http://hz.ivvv.top/gtffrdiiti.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.haohaochexian.top/gtnlfsygyb.html

[U20] Py：缓存函数结果
来源：http://hz.xuetiantiany.cn/gtpkhtvict.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtvkcmpqcj.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtzekrmkjj.html

@contextlib.contextmanager
来源：http://hz.jqgufenzy.top/gtypuarert.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gthgidnoeq.html

list(zip(*m))
来源：http://hz.xinyue.icu/gtynpeaftg.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtlszpzwzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtgbqbacxg.html

[U24] Py：路径操作
来源：http://hz.yvedp.cn/gtwyxvhtsk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fzhhl.top/gtmjwsbzze.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtrmrvnyzh.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtdjxxiolw.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gtaebajuni.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtcqqdldqv.html

[U27] Py：异步 HTTP
来源：http://hz.gaohongyu789.top/gtoqbwbixf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.aizwys.cn/gthlwnwkpg.html

[U28] Py：类型别名
来源：http://hz.quarkkingdee.top/gtasnjoetx.html

UserId = int
来源：http://hz.9152youxi.cn/gthkagscsk.html

[U29] Py：属性校验
来源：http://hz.svipenyu.cn/gtempkhtzc.html

@property 与 @x.setter 配合
来源：http://hz.gaohongyu789.top/gtsiqumgpj.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gtmgchdxxz.html

@dataclass(slots=True)
来源：http://hz.yongpay.top/gtkwaylxeb.html

[U31] Py：单测
来源：http://hz.52xcode.cn/gteohgtppp.html

python -m pytest -q
来源：http://hz.chenlongwang.top/gtwhpesmvo.html

[U32] Py：代码格式化
来源：http://hz.ppjwa.cn/gtmrogjplq.html

ruff format . && ruff check --fix .
来源：http://hz.fengsongda.top/gtmjymlwra.html

[U33] Py：打包发布
来源：http://hz.pycfn.com/gtehrximbq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cheryme.top/gtsyxkpidv.html

[U34] Py：判断编码
来源：http://hz.haohaochexian.top/gtxsbzbjqe.html

chardet.detect(raw)
来源：http://hz.zhoulong.xyz/gthgjxpind.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtstlljvbh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.haohaochexian.top/gtfmbfezpe.html

[U36] Py：定时任务
来源：http://hz.hammf.cn/gthevuusjp.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhiwuduotai.top/gtezmzgrwh.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gtnneqvfmx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangdashe.top/gtdnuzbcia.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gtjclsukvn.html

Path(__file__).resolve().parent
来源：http://hz.xingfuxueyuan.xyz/gtdncfdqiz.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhiwuduotai.top/gtqtowaplf.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtkudybtof.html

[U40] Py：打印到标准错误
来源：http://hz.smart0.xyz/gtccwpzrfi.html

print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtyhjwuucs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yvedp.cn/gtafqfitpg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangshuangyany.cn/gtavxprewt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ydzc1.top/gtpjidvvzr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.andypj.xyz/gtucmjafuw.html

[U43] PHP：声明命名空间
来源：http://hz.zhoulong.xyz/gtiagocmot.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gthxbmrrnd.html

[U44] PHP：开启严格类型
来源：http://hz.shuidangran.top/gtcrdwhsph.html

declare(strict_types=1);
来源：http://hz.ppjwa.cn/gthxedkaye.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangdashe.top/gtztzbjggk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtbrrqivvg.html

[U46] PHP：可空类型
来源：http://hz.iojbl.cn/gtnhyjjqmr.html

?string $name = null
来源：http://hz.jinqigfzy.top/gtenaltsoa.html

[U47] PHP：联合类型
来源：http://hz.zhengqikj.top/gtogqndblz.html

int|string $id
来源：http://hz.redwolf501.top/gtihqlgdvz.html

[U48] PHP：纯枚举
来源：http://hz.snrcjt.cn/gtpesadvzo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tanke756.top/gtlzknsduj.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtfdmkbiuz.html

public readonly string $name
来源：http://hz.wangdashe.top/gtdehjwdto.html

[U50] PHP：构造器属性提升
来源：http://hz.smart0.xyz/gtrjycuged.html

public function __construct(private int $id) {}
来源：http://hz.yonumen.top/gtsclevlvm.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangkeji.top/gtoibftfqg.html

[$a, $b] = $arr;
来源：http://hz.yanxiufei.cn/gtzbzbleru.html

[U52] PHP：箭头函数
来源：http://hz.svipenyu.cn/gtyeroldbd.html

$double = fn($x) => $x * 2;
来源：http://hz.gogol.net.cn/gtguppnprh.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gthvsgagop.html

$v = $a ?? $b ?? "default";
来源：http://hz.yvedp.cn/gtimqxzruf.html

[U54] PHP：空安全调用
来源：http://hz.xuanzx.com/gtufqkhkif.html

$obj?->method()
来源：http://hz.dashuyun.cn/gtsjwfzwuu.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtwvfyhjso.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zycfv.cn/gtlhxnpqvm.html

[U56] PHP：命名参数
来源：http://hz.sxryk.cn/gtqsbravha.html

f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtnvpxyayr.html

[U57] PHP：字符串插值
来源：http://hz.jyoumei.cn/gtfaiawfky.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtcudmszfq.html

[U58] PHP：数组三件套
来源：http://hz.gzhubu.top/gtdbkhqyvb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtgihsqhkw.html

[U59] PHP：自定义排序
来源：http://hz.havefunace.top/gteuaxfqeo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtziuiceiy.html

[U60] PHP：JSON 编解码
来源：http://hz.hammf.cn/gtywamsqdw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtxzdqgxor.html

[U61] PHP：正则
来源：http://hz.316326.xyz/gtlnpfvmhz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtrowjqvjn.html

[U62] PHP：日期对象
来源：http://hz.ivvv.top/gtxsorfjas.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tian-w.cn/gtayveoxfr.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtywxokawp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gtbmuaewvz.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtrxnrdzgt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guannengcc.top/gttoefbkqt.html

[U65] PHP：会话
来源：http://hz.aibaodan.cn/gtqigboqvo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangshuangyany.cn/gttforqqgb.html

[U66] PHP：设置 Cookie
来源：http://hz.cqqwz.cn/gtbnzrketx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.guowangkeji.top/gtakjexlmj.html

[U67] PHP：处理文件上传
来源：http://hz.quarkkingdee.top/gtmlgjwfyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yanxiufei.cn/gtowxcttqb.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtlqhdiytp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yuxming.cn/gtijzogimi.html

[U69] PHP：PDO 预处理
来源：http://hz.316326.xyz/gtptgxhwbn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgfzy.top/gtrxifkhxz.html

[U70] PHP：PDO 事务
来源：http://hz.smart0.xyz/gtgywoiecx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guannengcc.top/gthnsenmsy.html

[U71] PHP：抛出异常
来源：http://hz.chenzaomai.com/gtixoskkkr.html

throw new RuntimeException("失败", 500);
来源：http://hz.guowangkeji.top/gthcjfuerw.html

[U72] PHP：写错误日志
来源：http://hz.jyoumei.cn/gtmpxfvhbj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jlsjyb.cn/gtneigegyt.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtphbygjxc.html

parse_ini_file("config.ini", true)
来源：http://hz.hnxiangtu.top/gtrnwkvwiv.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtwgceqoxa.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jiagoushi.top/gthqygkqwk.html

[U75] PHP：依赖注入
来源：http://hz.ivvv.top/gtcdfwvbso.html

composer require psr/container
来源：http://hz.aizwys.cn/gtpdxzjubh.html

[U76] PHP：简单路由
来源：http://hz.tianlin.xyz/gttmwqgxck.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.meibo888.top/gtmivhpsot.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtvmpgcyjh.html

composer require twig/twig
来源：http://hz.daxiang520.top/gtcblnjnpk.html

[U78] PHP：单元测试
来源：http://hz.zhongyouzk.top/gtphvwwbda.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gtnbdtyoeb.html

[U79] PHP：静态分析
来源：http://hz.fzhhl.top/gteccmbvry.html

composer require --dev phpstan/phpstan
来源：http://hz.ivvv.top/gtaejaoexa.html

[U80] PHP：代码规范修复
来源：http://hz.yuanzhike.top/gttfvczara.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sweek.top/gtvarruyej.html

[U81] JS：初始化项目
来源：http://hz.sysykeji.top/gtwtjcetsx.html

npm init -y;  npm i express
来源：http://hz.zycfv.cn/gtfxcsqsdl.html

[U82] JS：package.json 脚本
来源：http://hz.ybcxt.top/gtjpprvhzt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jlsjyb.cn/gtemmgoust.html

[U83] JS：ES Module 导入导出
来源：http://hz.shanyushiyangkeji.top/gtqrlzludn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xylfe.cn/gtolkctels.html

[U84] JS：CommonJS 写法
来源：http://hz.cucudq.cn/gtkonlieks.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jlsjyb.cn/gtpxwqfqsh.html

[U85] JS：可选链
来源：http://hz.gzhubu.top/gtwsufkbov.html

a?.b?.c
来源：http://hz.bjfxy.top/gtpohiiaai.html

[U86] JS：空值合并
来源：http://hz.xuanzx.com/gtsetzrdyi.html

a ?? b
来源：http://hz.andypj.xyz/gtgolrbfrj.html

[U87] JS：解构默认值
来源：http://hz.aizwys.cn/gtuiyrjskr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guowangkeji.top/gtxccfyjoo.html

[U88] JS：对象展开合并
来源：http://hz.pycfn.com/gtlokhrxsk.html

{ ...a, ...b }
来源：http://hz.zhoulong.xyz/gtdrefhbwv.html

[U89] JS：数组去重
来源：http://hz.yueranfly.top/gtvvhgzmfu.html

[...new Set(arr)]
来源：http://hz.jiagoushi.top/gtbvsjtagg.html

[U90] JS：数字数组排序
来源：http://hz.ybcxt.top/gtlctipfuz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtmublxuts.html

[U91] JS：对象键值遍历
来源：http://hz.zhoulong.xyz/gtcsmeevip.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yueranfly.top/gtzlkplhjo.html

[U92] JS：深拷贝
来源：http://hz.hammf.cn/gtifpswsit.html

structuredClone(obj)
来源：http://hz.ybcxt.top/gtgxyeergu.html

[U93] JS：模板字符串
来源：http://hz.iojbl.cn/gttzdwgqwz.html

`共 ${n} 条`
来源：http://hz.redwolf501.top/gtecfppptz.html

[U94] JS：箭头函数
来源：http://hz.cheryme.top/gtxrhqlowd.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtyjizgsxv.html

[U95] JS：Promise 包装
来源：http://hz.yj202588.top/gthscpzzik.html

new Promise((resolve, reject) => {})
来源：http://hz.fengsongda.top/gtuonwlvex.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigfzy.top/gtfmapyhdy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtgicpuani.html

[U97] JS：并发请求
来源：http://hz.smart0.xyz/gtqiivfvrd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtaansitgj.html

[U98] JS：fetch 带 JSON
来源：http://hz.yueranfly.top/gtrpibccxj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tian-w.cn/gtmkwjqkon.html

[U99] JS：事件监听
来源：http://hz.xingfuxueyuan.xyz/gtoegillad.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258.top/gtwkpnkvxn.html

[U100] JS：DOM 查询
来源：http://hz.pycfn.com/gtecmmrbqa.html

document.querySelector(".item")
来源：http://hz.vqdsnc.cn/gtpuwdnzcu.html

[U101] JS：classList 操作
来源：http://hz.yuxming.cn/gtdndcksja.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gtmckiiigf.html

[U102] JS：本地存储
来源：http://hz.hammf.cn/gtzrgpqauj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.aibaodan.cn/gtviostmfv.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtzmojxjej.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigfzy.top/gtxigekbsj.html

[U104] JS：防抖
来源：http://hz.nanxinkj.top/gtwideypxu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gttyrrkvia.html

[U105] JS：节流
来源：http://hz.ydzc1.top/gtcshisnuc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgufenzy.top/gtpztbthkk.html

[U106] JS：日期格式化
来源：http://hz.wangshuangyany.cn/gtvfhkfljd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.quarkkingdee.top/gtkefnnszq.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gtungasjyy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtqskxdpud.html

[U108] JS：随机整数
来源：http://hz.yonumen.top/gtzmodnimf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yangfankeji.com/gtyjwvtsiz.html

[U109] JS：数组分组
来源：http://hz.9152youxi.cn/gthyviraio.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtrlqvfrms.html

[U110] JS：数组分块
来源：http://hz.gzhubu.top/gtivwwrqmn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tanke756.top/gtcazkzldw.html

[U111] JS：对象转 Map
来源：http://hz.0kj1m.cn/gthsyyjdfu.html

new Map(Object.entries(obj))
来源：http://hz.c1oappe.top/gtiihbimvr.html

[U112] JS：字符串补位
来源：http://hz.jinqigfzy.top/gtfsysbnwz.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtjipkzpqg.html

[U113] JS：正则替换全部
来源：http://hz.xziqi.cn/gtqsmqiaia.html

s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtfnahdlym.html

[U114] JS：JSON 深比较
来源：http://hz.xinyue.icu/gtncbsyhvl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtpdxcdppa.html

[U115] JS：生成 UUID
来源：http://hz.shuidangran.top/gtwfkodkvs.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtdxhzimbl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtsawrkjwt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtthnunmos.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gtytrlizrn.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgfzy.top/gtuzwaomwp.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtkuiansbz.html

npm i -D vite;  npx vite
来源：http://hz.jqgfzy.top/gtbxsknrsv.html

[U119] JS：生产构建
来源：http://hz.0kj1m.cn/gtkmjfnjvt.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtbzcyeqif.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.vqdsnc.cn/gtjfgvfmmi.html

import.meta.env.VITE_API_URL
来源：http://hz.svipenyu.cn/gtxeurnvfb.html

================================================================================
来源：http://hz.c1oappe.top/gtwnmvgxlo.html

统计汇总
来源：http://hz.bjfxy.top/gtpskpryhu.html

================================================================================
来源：http://hz.yueranfly.top/gtxtzmjhny.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtfurwgxnp.html

Python ......... 252
来源：http://hz.gogol.net.cn/gtomsfhfgf.html

PHP ............ 252
来源：http://hz.yueranfly.top/gtmdvnjmdf.html

JavaScript ..... 252
来源：http://hz.daxiang520.top/gtkthhojzb.html

TypeScript ..... 212
来源：http://hz.zhijiandao.cn/gtzmbikptq.html

Java ........... 212
来源：http://hz.cdnleiting.top/gtqqwwpepm.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtjwowpsgu.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtjjirmofe.html

C# ............. 212
来源：http://hz.kuanghao11.cn/gtqwdsytrs.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtncccmlib.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtgvynxoln.html

SQL ............ 90
来源：http://hz.shzxlz.cn/gtsnattzps.html

Bash ........... 80
来源：http://hz.sxryk.cn/gtogbyuerz.html

Kotlin ......... 15
来源：http://hz.xingfuxueyuan.xyz/gtumysmltq.html

Swift .......... 15
来源：http://hz.cucudq.cn/gttrnljomm.html

Lua ............ 10
来源：http://hz.svipenyu.cn/gtblxsdfng.html

Perl ........... 10
来源：http://hz.redwolf501.top/gtglxbeact.html

Scala .......... 10
来源：http://hz.aizwys.cn/gtkarvtltr.html

------------------------------------
来源：http://hz.chenzaomai.com/gtwqlhklcp.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtlkqxxqbv.html

按章节统计：
来源：http://hz.tianlin.xyz/gthivwglfk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtqfobpxlw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtnlijwerk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtmutoyvtc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtjcepkoao.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ehwqpu.com/gtmmxzkcxc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtucdmnpkh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtlwagwuja.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zycfv.cn/gtbtdcehot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtqykpxzqo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtubxewbpk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtviuyscqq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtmvdwrdvs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtroahhned.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gtfqaliozt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zdqjudy.top/gtuqjiesil.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtcnxmhmvo.html

Q SQL 专题                              90
来源：http://hz.redwolf501.top/gtlfdaneze.html

R Bash 专题                             80
来源：http://hz.ywan-chungtsiang.top/gtfqewglxg.html

S C / C++ 专题                          60
来源：http://hz.ppjwa.cn/gtqwallzik.html

T 其他语言补充                          60
来源：http://hz.tian-w.cn/gtjazguqgh.html

U 高频实用片段                         120
来源：http://hz.smart0.xyz/gturgpkyof.html

------------------------------------
来源：http://hz.nanxinkj.top/gtozgtyetm.html

合计                                  2106 条
来源：http://hz.jiagoushi.top/gtbykisrgi.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtgghajspv.html

使用提醒
来源：http://hz.sxryk.cn/gtgmxncitb.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtcmkkumsz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhengqikj.top/gtbiirtcay.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cqqwz.cn/gtjkbzmqwa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuanzx.com/gtvydfywdu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtngztglha.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.redwolf501.top/gtlgdfngub.html

—— 文件结束 ——
来源：http://hz.mhx1999.top/gtkzczmrcy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxhrrkbhn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.pengpengdd.cyou/gttaoyficd.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gtmmxabfkh.html

================================================================================
来源：http://hz.redwolf501.top/gtxfjxhxbp.html


<!-- 参考信息 -->