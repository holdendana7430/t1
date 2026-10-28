代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hz.yj202588.top/gtczwiksap.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cucudq.cn/gtxheablzc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtwrdkhlgx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cashguo.top/gtmtcjoeti.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gtjrzxdhdf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigufen.top/gtyoybhcin.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangtech.top/gtsaxdxebf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhixingplan.top/gtylownosf.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtvyqlsaus.html

list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtunlfvfca.html

[U06] Py：合并两个字典
来源：http://hz.tian-w.cn/gtstrkpsmx.html

{**a, **b}
来源：http://hz.gaohongyu789.top/gtlclcxlsi.html

[U07] Py：反转字典键值
来源：http://hz.9152youxi.cn/gtkchjrmsu.html

{v: k for k, v in d.items()}
来源：http://hz.chenzaomai.com/gtnbxzjwmi.html

[U08] Py：展平二维列表
来源：http://hz.zdqjudy.top/gtdiabidrl.html

[y for x in nested for y in x]
来源：http://hz.hysaishi.cn/gtmqrfkedm.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtbmxxmdls.html

max(d, key=d.get)
来源：http://hz.zhaomingkeji.xyz/gttsjvnyzq.html

[U10] Py：按值排序字典
来源：http://hz.jqgufenzy.top/gtkolblpbv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xingfuxueyuan.xyz/gtmuyxmzmi.html

[U11] Py：生成器表达式
来源：http://hz.chenjidiqi.icu/gtatdkqnyu.html

(x * 2 for x in arr)
来源：http://hz.vqdsnc.cn/gtsovabqfi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jianghu66.top/gtdrmxxblh.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtzzvcejub.html

[U13] Py：固定长度队列
来源：http://hz.zhijiandao.cn/gthibiusfn.html

deque(maxlen=10)
来源：http://hz.shzxlz.cn/gtwvtqgdkc.html

[U14] Py：分组收集到列表
来源：http://hz.cheryme.top/gtmowsxmbq.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtjeeufjkz.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtncsmuspd.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gtjinhpnjr.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtsmlsnpum.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhongyouzk.top/gtjqihnrzt.html

[U17] Py：初始化日志
来源：http://hz.shangyingyoupin.top/gtztotvdoy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.316326.xyz/gtdtgtzfkb.html

[U18] Py：预编译正则
来源：http://hz.redwolf501.top/gtvmrxwwtm.html

pat = re.compile(r"\d+")
来源：http://hz.aizwys.cn/gtzrjuycbc.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtfevsrbbk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dianchejie.cn/gtkquzpfeo.html

[U20] Py：缓存函数结果
来源：http://hz.cucudq.cn/gtwppahfby.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtqdctuyun.html

[U21] Py：自定义上下文管理器
来源：http://hz.andypj.xyz/gtcrwhwywo.html

@contextlib.contextmanager
来源：http://hz.0kj1m.cn/gtsgliiyyh.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gtwneggvlo.html

list(zip(*m))
来源：http://hz.gotoacloud.top/gtebehpwxi.html

[U23] Py：分块读取大文件
来源：http://hz.yuanzhike.top/gtimowaaet.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhixingplan.top/gtmqawslqn.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gtebrvwrel.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.aizwys.cn/gthiynbgcv.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258.top/gteajhnrxl.html

csv.DictReader(f)
来源：http://hz.chenzaomai.com/gtvkbxinjy.html

[U26] Py：并发下载
来源：http://hz.wangdashe.top/gtcxbaoskn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtvqssoywd.html

[U27] Py：异步 HTTP
来源：http://hz.shanyushiyangkeji.top/gteytetobi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gzhubu.top/gttmulwmvw.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gtcinqtzfo.html

UserId = int
来源：http://hz.gzhubu.top/gtlrkyrirs.html

[U29] Py：属性校验
来源：http://hz.zhaomingkeji.xyz/gttvcdajlr.html

@property 与 @x.setter 配合
来源：http://hz.jqgfzy.top/gttexqhrst.html

[U30] Py：数据类
来源：http://hz.kuanghao11.cn/gtdjhuhesn.html

@dataclass(slots=True)
来源：http://hz.redwolf501.top/gtgnwglvbd.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gtrfvkzxst.html

python -m pytest -q
来源：http://hz.jlsjyb.cn/gtlssfowgw.html

[U32] Py：代码格式化
来源：http://hz.aizwys.cn/gtbuedsyax.html

ruff format . && ruff check --fix .
来源：http://hz.yonumen.top/gtluofptus.html

[U33] Py：打包发布
来源：http://hz.daria6918.cn/gtkewkpnlo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hnxiangtu.top/gtltgpasbi.html

[U34] Py：判断编码
来源：http://hz.nanxuanxn.top/gtdpzhaqfx.html

chardet.detect(raw)
来源：http://hz.jinghuilouyu.cn/gtmtdjqlni.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangtech.top/gtdccezmbm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tanke756.top/gtbtgghidt.html

[U36] Py：定时任务
来源：http://hz.c1oappe.top/gtxytjuiev.html

schedule.every(10).minutes.do(job)
来源：http://hz.vqdsnc.cn/gtyzecpvsq.html

[U37] Py：读写 Excel
来源：http://hz.jqgufenzy.top/gtkbyfmlgs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuetiantiany.cn/gtjwsquodc.html

[U38] Py：获取脚本所在目录
来源：http://hz.smart0.xyz/gthdszabgr.html

Path(__file__).resolve().parent
来源：http://hz.ivvv.top/gtcipnozqu.html

[U39] Py：判断是否在交互环境
来源：http://hz.yvedp.cn/gtmzdqcpcv.html

sys.stdout.isatty()
来源：http://hz.zhengqikj.top/gtqqxmgmjx.html

[U40] Py：打印到标准错误
来源：http://hz.shuidangran.top/gttttpnmwg.html

print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gttmszjswm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxinkj.top/gtgorqrizq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yj20258888.top/gttiakmrwl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gteqjukdrv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.0kj1m.cn/gtcxagwmey.html

[U43] PHP：声明命名空间
来源：http://hz.xingfuxueyuan.xyz/gtssrnnxpg.html

namespace App\Http;
来源：http://hz.c1oappe.top/gteofikaji.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gthhxfbklr.html

declare(strict_types=1);
来源：http://hz.shzxlz.cn/gtewxgboyo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhoulong.xyz/gtkjoieuzp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.kuanghao11.cn/gtpftalxyk.html

[U46] PHP：可空类型
来源：http://hz.ydzc1.top/gthlcmptfx.html

?string $name = null
来源：http://hz.ydjk.org.cn/gtblrteklu.html

[U47] PHP：联合类型
来源：http://hz.meibo888.top/gtpszsivwr.html

int|string $id
来源：http://hz.chenzaomai.com/gtbigwibic.html

[U48] PHP：纯枚举
来源：http://hz.zdqjudy.top/gtjbduchgz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.haohaochexian.top/gtovssfieu.html

[U49] PHP：只读属性
来源：http://hz.tian-w.cn/gtiqufyifi.html

public readonly string $name
来源：http://hz.sysykeji.top/gtsamcfdew.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258888.top/gthbckxluc.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtfumuxqzb.html

[U51] PHP：数组解构
来源：http://hz.hnxiangtu.top/gtizigegnl.html

[$a, $b] = $arr;
来源：http://hz.zhaomingkeji.xyz/gttufaejdd.html

[U52] PHP：箭头函数
来源：http://hz.cqqwz.cn/gtdiuvsuui.html

$double = fn($x) => $x * 2;
来源：http://hz.mhx1999.top/gtuxmerujl.html

[U53] PHP：空合并运算符
来源：http://hz.zhengqikj.top/gtynttkrrs.html

$v = $a ?? $b ?? "default";
来源：http://hz.yongpay.top/gtfjfpiape.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtbhbidmdb.html

$obj?->method()
来源：http://hz.iojbl.cn/gtptwrkhdh.html

[U55] PHP：match 表达式
来源：http://hz.shangyingyoupin.top/gtqryyfrps.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cashguo.top/gtikqtnpak.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtighcjdzh.html

f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtbuwlqtpy.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gthblwweut.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtequwtmez.html

[U58] PHP：数组三件套
来源：http://hz.0kj1m.cn/gtmxanhioj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigfzy.top/gtcyqynkak.html

[U59] PHP：自定义排序
来源：http://hz.feifeiyinyue.top/gtylcxnmhr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtrpnrxuly.html

[U60] PHP：JSON 编解码
来源：http://hz.sxryk.cn/gtcxthdkqc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.daxiang520.top/gtilsmgafn.html

[U61] PHP：正则
来源：http://hz.wangshuangyany.cn/gtqaqllfuk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gthixrvecp.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtgrlvbnsj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gtomubtoom.html

[U63] PHP：文件读写
来源：http://hz.zhaomingkeji.xyz/gthnasiryz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gotoacloud.top/gtkukmosca.html

[U64] PHP：目录遍历
来源：http://hz.wangshuangyany.cn/gtimcfnail.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangkeji.top/gtaorxsmrs.html

[U65] PHP：会话
来源：http://hz.shanyushiyangtech.top/gtrnczkjin.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shzxlz.cn/gtokaugjmy.html

[U66] PHP：设置 Cookie
来源：http://hz.sweek.top/gtcqzsuxhj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.feifeiyinyue.top/gtsawhhnyu.html

[U67] PHP：处理文件上传
来源：http://hz.haohaochexian.top/gtglfypnki.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.vqdsnc.cn/gtyrxkrwjg.html

[U68] PHP：PDO 连接
来源：http://hz.dashuyun.cn/gtqzxpebml.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gzhubu.top/gtrghddrce.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtifpqjeqf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuxming.cn/gtgbmtzrda.html

[U70] PHP：PDO 事务
来源：http://hz.yongpay.top/gthgcdrcxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtyfvrnitv.html

[U71] PHP：抛出异常
来源：http://hz.snrcjt.cn/gtgcpnphea.html

throw new RuntimeException("失败", 500);
来源：http://hz.redwolf501.top/gtctervbif.html

[U72] PHP：写错误日志
来源：http://hz.iojbl.cn/gtqmrjgqij.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gaohongyu789.top/gtsvbhwjkf.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtyyjlimdg.html

parse_ini_file("config.ini", true)
来源：http://hz.sweek.top/gttcukasii.html

[U74] PHP：读取环境变量
来源：http://hz.c1oappe.top/gtorvhyxgn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtipqcqnfi.html

[U75] PHP：依赖注入
来源：http://hz.hysaishi.cn/gttnxbbrey.html

composer require psr/container
来源：http://hz.fzhhl.top/gtsjjpdcng.html

[U76] PHP：简单路由
来源：http://hz.xuanzx.com/gtbiusqevk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ydjk.org.cn/gtqdgmdesa.html

[U77] PHP：模板渲染
来源：http://hz.tianlin.xyz/gtexjnqblg.html

composer require twig/twig
来源：http://hz.tian-w.cn/gtlgtqvvyv.html

[U78] PHP：单元测试
来源：http://hz.zhijiandao.cn/gthzdvgdbl.html

composer require --dev phpunit/phpunit
来源：http://hz.zhengqikj.top/gtvrvxckji.html

[U79] PHP：静态分析
来源：http://hz.chenjidiqi.icu/gtbhluzzlp.html

composer require --dev phpstan/phpstan
来源：http://hz.sysykeji.top/gtlvpufopa.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtnlrhjqro.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangshuangyany.cn/gtthdsdeir.html

[U81] JS：初始化项目
来源：http://hz.yuanzhike.top/gtkhiygulj.html

npm init -y;  npm i express
来源：http://hz.zhongyouzk.top/gtvrpcqsic.html

[U82] JS：package.json 脚本
来源：http://hz.hnxiangtu.top/gtnflederc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtfbospjof.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydzc1.top/gtasolayfb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258888.top/gtscriohpw.html

[U84] JS：CommonJS 写法
来源：http://hz.zycfv.cn/gtqqshzzek.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.andypj.xyz/gtwdmcyqqk.html

[U85] JS：可选链
来源：http://hz.zhiwuduotai.top/gtzdkelbjh.html

a?.b?.c
来源：http://hz.jlsjyb.cn/gtssxpyhad.html

[U86] JS：空值合并
来源：http://hz.ydzc1.top/gtwrmjlbbe.html

a ?? b
来源：http://hz.yvedp.cn/gtnhqpnbtj.html

[U87] JS：解构默认值
来源：http://hz.redwolf501.top/gtebgcsmsl.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtrmmsenhe.html

[U88] JS：对象展开合并
来源：http://hz.sufxvd.cn/gtvxstfrqy.html

{ ...a, ...b }
来源：http://hz.c1oappe.top/gtbscgsimn.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gttjezgndx.html

[...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtmoirypdh.html

[U90] JS：数字数组排序
来源：http://hz.jinqigufen.top/gttkdscypz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtrgwbsuxz.html

[U91] JS：对象键值遍历
来源：http://hz.bjfxy.top/gtakbqkugu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guowangkeji.top/gtuzjnibhw.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gtssfngsox.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtmergbfac.html

[U93] JS：模板字符串
来源：http://hz.tian-w.cn/gtfivbjard.html

`共 ${n} 条`
来源：http://hz.andypj.xyz/gtfckypthk.html

[U94] JS：箭头函数
来源：http://hz.shuidangran.top/gtlggzfsiv.html

const double = x => x * 2;
来源：http://hz.jiagoushi.top/gtoiydbwtb.html

[U95] JS：Promise 包装
来源：http://hz.gzhubu.top/gtcfmlesib.html

new Promise((resolve, reject) => {})
来源：http://hz.havefunace.top/gtkxkqvjrv.html

[U96] JS：async/await 与异常
来源：http://hz.jianghu66.top/gtofnxvhfn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtdfwhjxvb.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtgldhevpj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtvfumxovu.html

[U98] JS：fetch 带 JSON
来源：http://hz.gotoacloud.top/gtjaikhhlm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.andypj.xyz/gtzgmjcska.html

[U99] JS：事件监听
来源：http://hz.meibo888.top/gtrjfeguhb.html

el.addEventListener("click", e => {})
来源：http://hz.hammf.cn/gtpodabboe.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtuhnvzkue.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gttmswcvee.html

[U101] JS：classList 操作
来源：http://hz.yj20258.top/gtgmqnrxcn.html

el.classList.toggle("active")
来源：http://hz.jqgufenzy.top/gtetitvwsi.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtxtkbjaxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangshuangyany.cn/gtggmjwscx.html

[U103] JS：定时器
来源：http://hz.jinyuanbaomall.cn/gtmjeaqwsy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.feifeiyinyue.top/gtbwmtfvpe.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtzjfpwstr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtwdxejocd.html

[U105] JS：节流
来源：http://hz.birdmap.top/gtgecfothc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gzhubu.top/gtiannhgda.html

[U106] JS：日期格式化
来源：http://hz.andypj.xyz/gtjbqvrtih.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yonumen.top/gtrceggdcc.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtsvubyznx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gtkwkhwpem.html

[U108] JS：随机整数
来源：http://hz.fzhhl.top/gtnmbswhkk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydzc1.top/gtwgcxgvit.html

[U109] JS：数组分组
来源：http://hz.tianlin.xyz/gtxynhfvet.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtqwurzmwb.html

[U110] JS：数组分块
来源：http://hz.zhixingplan.top/gtqntquwio.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dianchejie.cn/gtdjeegfxh.html

[U111] JS：对象转 Map
来源：http://hz.cucudq.cn/gtsbggeste.html

new Map(Object.entries(obj))
来源：http://hz.yangfankeji.com/gtetavplvs.html

[U112] JS：字符串补位
来源：http://hz.jinqigufen.top/gtgjeidpog.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtyugdvjhu.html

[U113] JS：正则替换全部
来源：http://hz.havefunace.top/gtgiahbxho.html

s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtztqpjxdy.html

[U114] JS：JSON 深比较
来源：http://hz.ehwqpu.com/gtrsaicpta.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtxjorbeyf.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gtgyjmdsfc.html

crypto.randomUUID()
来源：http://hz.birdmap.top/gtrdlbljni.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.quarkkingdee.top/gtmhmftalh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtdwspgynl.html

[U117] JS：单元测试
来源：http://hz.kuanghao11.cn/gtsivlfuyk.html

npm i -D vitest;  npx vitest
来源：http://hz.316326.xyz/gtzoesdpyo.html

[U118] JS：开发服务器
来源：http://hz.sysykeji.top/gtvsfspwed.html

npm i -D vite;  npx vite
来源：http://hz.zhixingplan.top/gttktpnerj.html

[U119] JS：生产构建
来源：http://hz.hnxiangtu.top/gtyrbbwqkd.html

npx vite build
来源：http://hz.jinghuilouyu.cn/gtxuxjlere.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhoulong.xyz/gtkcybtobq.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258.top/gtkdfordvs.html

================================================================================
来源：http://hz.tianlin.xyz/gtabfnqszx.html

统计汇总
来源：http://hz.yvedp.cn/gtlwuhryhr.html

================================================================================
来源：http://hz.ivvv.top/gtwnqdlecc.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gttbhsbvva.html

Python ......... 252
来源：http://hz.cucudq.cn/gticjdgtyq.html

PHP ............ 252
来源：http://hz.jqgufenzy.top/gtbedquydp.html

JavaScript ..... 252
来源：http://hz.zhixingplan.top/gtixpcpilt.html

TypeScript ..... 212
来源：http://hz.hnxiangtu.top/gtqljvffrv.html

Java ........... 212
来源：http://hz.smart0.xyz/gtbbtnxvez.html

Go ............. 212
来源：http://hz.cdnleiting.top/gttqxyvxdm.html

Ruby ........... 212
来源：http://hz.zhongyouzk.top/gthueqfwub.html

C# ............. 212
来源：http://hz.birdmap.top/gtycmnwhou.html

C .............. 30
来源：http://hz.yongpay.top/gtliwmyyrd.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gtyfkllzov.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gtaxsxiulr.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtjhzqrqss.html

Kotlin ......... 15
来源：http://hz.sysykeji.top/gtmacihpja.html

Swift .......... 15
来源：http://hz.iojbl.cn/gtydfxeiss.html

Lua ............ 10
来源：http://hz.cheryme.top/gtxalkozgv.html

Perl ........... 10
来源：http://hz.havefunace.top/gtpswlloty.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtalyzyado.html

------------------------------------
来源：http://hz.tianlin.xyz/gtkimtcxzi.html

合计 ........... 2106 条
来源：http://hz.cashguo.top/gtmtuefyoj.html

按章节统计：
来源：http://hz.andypj.xyz/gtalggbotr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtvdnlafzp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtjcyspmug.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtmoldquud.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gtauacqehc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuanzhike.top/gttkhnswmx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ydzc1.top/gttgktlpnl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtzgwpbdxs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtcisgyqyk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtthqpwvfb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtlcgmfgvu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtbbwzqpjb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtzvzjbxsk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtclbdjfye.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtslyqotpd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sysykeji.top/gtkjnplqoq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtedoheusl.html

Q SQL 专题                              90
来源：http://hz.cqqwz.cn/gtsljhrxzk.html

R Bash 专题                             80
来源：http://hz.fzhhl.top/gtllvumwwj.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtjvyfsskf.html

T 其他语言补充                          60
来源：http://hz.shanyushiyangtech.top/gtdrstsjag.html

U 高频实用片段                         120
来源：http://hz.snrcjt.cn/gtbhjoohmt.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtfsxrkhwq.html

合计                                  2106 条
来源：http://hz.andypj.xyz/gtxpvtlljh.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gttnczgnti.html

使用提醒
来源：http://hz.andypj.xyz/gtbfvhrdlq.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtcfqhezaq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydjk.org.cn/gtaajkjwny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinghuilouyu.cn/gtugnvdmgt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yuanzhike.top/gtcgbmbgxt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhijiandao.cn/gtzfpqwvgi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangdashe.top/gtbeumnbsr.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtkvwdrqld.html

================================================================================
来源：http://hz.zycfv.cn/gthxeembzo.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jianghu66.top/gtaghtklre.html

Common Programming Examples Cheat Book
来源：http://hz.c1oappe.top/gtzpvbxwio.html

================================================================================
来源：http://hz.hywenlv.cn/gtehhnzahp.html


<!-- 参考信息 -->