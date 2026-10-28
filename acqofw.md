代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhaomingkeji.xyz/gtujwgbtup.html

================================================================================
来源：http://hz.zdqjudy.top/gtbwldomgz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ppjwa.cn/gtqwzyualp.html

================================================================================
来源：http://hz.yuxming.cn/gtnptxmmfq.html

[U01] Py：创建虚拟环境
来源：http://hz.zhongyouzk.top/gtldnyqhdk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.vqdsnc.cn/gtcaeheclt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hysaishi.cn/gtmkjllsus.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jianghu66.top/gtnocrktxw.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtfyvclwhi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.snrcjt.cn/gtwcjfsmof.html

[U04] Py：变量调试打印
来源：http://hz.aizwys.cn/gtwgwuwzyu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuanzx.com/gtcymhqrgc.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtibuqnzoo.html

list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtzbmfminv.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gtqykxngnt.html

{**a, **b}
来源：http://hz.0kj1m.cn/gtsdptokxv.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gtzmryknvp.html

{v: k for k, v in d.items()}
来源：http://hz.xinyue.icu/gtfugprhrg.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gtsyeyqrbl.html

[y for x in nested for y in x]
来源：http://hz.zhoulong.xyz/gtcopobaaw.html

[U09] Py：字典取最大值的键
来源：http://hz.guowangkeji.top/gtijzopvvp.html

max(d, key=d.get)
来源：http://hz.jinqigufen.top/gtmlsvivtf.html

[U10] Py：按值排序字典
来源：http://hz.zhengqikj.top/gtzgaieawf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtddbiveho.html

[U11] Py：生成器表达式
来源：http://hz.sysykeji.top/gtsosqonow.html

(x * 2 for x in arr)
来源：http://hz.ivvv.top/gtftddjrer.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gtavnryhuk.html

Counter(arr).most_common(3)
来源：http://hz.wangshuangyany.cn/gtflyiifao.html

[U13] Py：固定长度队列
来源：http://hz.chenlongwang.top/gtjnuukvpb.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gtfczsxrzx.html

[U14] Py：分组收集到列表
来源：http://hz.yongpay.top/gtyzcpetxw.html

defaultdict(list)
来源：http://hz.birdmap.top/gtynityprz.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtvbnjsxcn.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtuhrpwjpb.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtpbghgrrj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxinkj.top/gttnonqiql.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtomrozmhe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cucudq.cn/gtlmzjgkoq.html

[U18] Py：预编译正则
来源：http://hz.c1oappe.top/gtzucsphim.html

pat = re.compile(r"\d+")
来源：http://hz.havefunace.top/gtxwvrhskl.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gtovtltyzk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guowangkeji.top/gttwpfguqm.html

[U20] Py：缓存函数结果
来源：http://hz.vqdsnc.cn/gtwnplgimw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xziqi.cn/gtvwhliywc.html

[U21] Py：自定义上下文管理器
来源：http://hz.sysykeji.top/gtovbptdwg.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gteqyxseuc.html

[U22] Py：矩阵转置
来源：http://hz.shangyingyoupin.top/gtgytcllct.html

list(zip(*m))
来源：http://hz.316326.xyz/gtyuglheuv.html

[U23] Py：分块读取大文件
来源：http://hz.feifeiyinyue.top/gtehebefdx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgfzy.top/gtevyqvgnf.html

[U24] Py：路径操作
来源：http://hz.yanxiufei.cn/gtqelgxrjy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtfpiqtatc.html

[U25] Py：CSV 按字典读
来源：http://hz.jlsjyb.cn/gtcjzzbjji.html

csv.DictReader(f)
来源：http://hz.yongpay.top/gtwnwapeoo.html

[U26] Py：并发下载
来源：http://hz.cdnleiting.top/gtmsfjbjee.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hfpthk.cn/gtafubrkjz.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtdbwzukww.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.c1oappe.top/gtqrkwggmk.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtzdqfkbpz.html

UserId = int
来源：http://hz.jqgufenzy.top/gtifpihoiv.html

[U29] Py：属性校验
来源：http://hz.ivvv.top/gtwmpfwbfi.html

@property 与 @x.setter 配合
来源：http://hz.nanxinkj.top/gtvkfiquxg.html

[U30] Py：数据类
来源：http://hz.zhongyouzk.top/gtzpjjegsk.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtjprlmxol.html

[U31] Py：单测
来源：http://hz.birdmap.top/gthifjvpsu.html

python -m pytest -q
来源：http://hz.guowangkeji.top/gtnywkfrtq.html

[U32] Py：代码格式化
来源：http://hz.gaohongyu789.top/gtjtrtvvap.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gtekdshkut.html

[U33] Py：打包发布
来源：http://hz.smart0.xyz/gtxohloiyk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtczafvrsm.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gtdvdrrnti.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtsodttmot.html

[U35] Py：发送邮件
来源：http://hz.tianlin.xyz/gtbfjakvso.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhaomingkeji.xyz/gtuavgestr.html

[U36] Py：定时任务
来源：http://hz.cheryme.top/gthurwjirm.html

schedule.every(10).minutes.do(job)
来源：http://hz.daria6918.cn/gtvnirsuem.html

[U37] Py：读写 Excel
来源：http://hz.zhengqikj.top/gtfxclfsfx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.c1oappe.top/gtqzfufeaq.html

[U38] Py：获取脚本所在目录
来源：http://hz.yonumen.top/gtrazaqomv.html

Path(__file__).resolve().parent
来源：http://hz.yj20258888.top/gtrtfvcyhp.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtbxwdorxr.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtwhqnbsvk.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gtrakvxoom.html

print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtisbgkplo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnxiangtu.top/gtzuoekcao.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gtsjrwnbgi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtergzstsz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.316326.xyz/gtxbhbprlc.html

[U43] PHP：声明命名空间
来源：http://hz.nanxuanxn.top/gthajmrsxg.html

namespace App\Http;
来源：http://hz.smart0.xyz/gtyacnfzny.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtleasalop.html

declare(strict_types=1);
来源：http://hz.jiagoushi.top/gtzitwbrks.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ppjwa.cn/gtlkyyiexo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtawsputdv.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtepkswkfy.html

?string $name = null
来源：http://hz.chenlongwang.top/gtautqnxls.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtdiltpswf.html

int|string $id
来源：http://hz.sweek.top/gtwdpxiqtx.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtdtijqxlr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangdashe.top/gtbxczrnvv.html

[U49] PHP：只读属性
来源：http://hz.iojbl.cn/gtnkruphem.html

public readonly string $name
来源：http://hz.shangyingyoupin.top/gtxbkxzamc.html

[U50] PHP：构造器属性提升
来源：http://hz.nwbrower.top/gtjtxgeeoc.html

public function __construct(private int $id) {}
来源：http://hz.zhengqikj.top/gteoebjbhh.html

[U51] PHP：数组解构
来源：http://hz.yueranfly.top/gtljlzsnmm.html

[$a, $b] = $arr;
来源：http://hz.cucudq.cn/gthsxxbfgh.html

[U52] PHP：箭头函数
来源：http://hz.ivvv.top/gtkgkzgzcg.html

$double = fn($x) => $x * 2;
来源：http://hz.mhx1999.top/gtfhccsnhv.html

[U53] PHP：空合并运算符
来源：http://hz.zhixingplan.top/gtgrhwrpzt.html

$v = $a ?? $b ?? "default";
来源：http://hz.fengsongda.top/gtivouibcl.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtpepdupeo.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtkjyktedz.html

[U55] PHP：match 表达式
来源：http://hz.yongpay.top/gtosvrqmvm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtjvxpugze.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtlnmypluj.html

f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtqdsayytq.html

[U57] PHP：字符串插值
来源：http://hz.zhongyouzk.top/gtxvqmglrf.html

"值: {$a}"
来源：http://hz.hongshengwenyu.top/gthjincrvv.html

[U58] PHP：数组三件套
来源：http://hz.nanxinkj.top/gtaapwiohh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhengqikj.top/gtjgqsjquq.html

[U59] PHP：自定义排序
来源：http://hz.gzhubu.top/gtbvsvfcxp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtdggbiupj.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgufenzy.top/gtkxfrbeix.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.wangshuangyany.cn/gtbtjeavlv.html

[U61] PHP：正则
来源：http://hz.redwolf501.top/gtknxgxsth.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gturllvhoo.html

[U62] PHP：日期对象
来源：http://hz.ybcxt.top/gtpithzgdz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gzhubu.top/gtodajhtty.html

[U63] PHP：文件读写
来源：http://hz.hammf.cn/gtpwnymemz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aizwys.cn/gtkivsregm.html

[U64] PHP：目录遍历
来源：http://hz.andypj.xyz/gtvzkdmxbv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shangyingyoupin.top/gtnliacaxx.html

[U65] PHP：会话
来源：http://hz.aibaodan.cn/gtxdxpgwib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuxming.cn/gtyqdcwhtn.html

[U66] PHP：设置 Cookie
来源：http://hz.yj20258.top/gtgdkdomkv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ybcxt.top/gtylzjihbq.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtenwtrqmt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gaohongyu789.top/gtwhdsthfl.html

[U68] PHP：PDO 连接
来源：http://hz.jianghu66.top/gtbnofefjq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhiwuduotai.top/gtbkalmwqg.html

[U69] PHP：PDO 预处理
来源：http://hz.zhiwuduotai.top/gtlvuifbgb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.andypj.xyz/gtdcskahcq.html

[U70] PHP：PDO 事务
来源：http://hz.316326.xyz/gtlerzcvua.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sxryk.cn/gtqlyrcigi.html

[U71] PHP：抛出异常
来源：http://hz.hfpthk.cn/gtpblujzyz.html

throw new RuntimeException("失败", 500);
来源：http://hz.xziqi.cn/gtmeztxkck.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtrfyyuetp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cdnleiting.top/gtpocpxhef.html

[U73] PHP：读取 ini 配置
来源：http://hz.hysaishi.cn/gtgjxrikah.html

parse_ini_file("config.ini", true)
来源：http://hz.jinyuanbaomall.cn/gtkgnrmmkt.html

[U74] PHP：读取环境变量
来源：http://hz.gogol.net.cn/gtriclpnig.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenlongwang.top/gtjisgjjxd.html

[U75] PHP：依赖注入
来源：http://hz.gogol.net.cn/gtfgbxpsgl.html

composer require psr/container
来源：http://hz.gotoacloud.top/gtedsatypx.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangtech.top/gtpmcfaacj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtkseqeklt.html

[U77] PHP：模板渲染
来源：http://hz.nanxinkj.top/gtcyjehkib.html

composer require twig/twig
来源：http://hz.snrcjt.cn/gtvpyhfkcs.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtaujxbfvy.html

composer require --dev phpunit/phpunit
来源：http://hz.dianchejie.cn/gtcymrlbvo.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtavfjqqui.html

composer require --dev phpstan/phpstan
来源：http://hz.jyoumei.cn/gtmxwlhnir.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gthbgxmnci.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cdnleiting.top/gtvnqruudo.html

[U81] JS：初始化项目
来源：http://hz.redwolf501.top/gtnbnodsff.html

npm init -y;  npm i express
来源：http://hz.tanke756.top/gtlcgoqmdi.html

[U82] JS：package.json 脚本
来源：http://hz.wangshuangyany.cn/gtybmatvof.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gzhubu.top/gthdrnnjfe.html

[U83] JS：ES Module 导入导出
来源：http://hz.9152youxi.cn/gtziobktwg.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xuanzx.com/gthhglyhwb.html

[U84] JS：CommonJS 写法
来源：http://hz.cheryme.top/gtuqlojzpp.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenlongwang.top/gtojunwnql.html

[U85] JS：可选链
来源：http://hz.jqgfzy.top/gtdftuvymv.html

a?.b?.c
来源：http://hz.andypj.xyz/gtbcpbjdet.html

[U86] JS：空值合并
来源：http://hz.jiagoushi.top/gtfavhmpkb.html

a ?? b
来源：http://hz.cqqwz.cn/gtfnhnvljb.html

[U87] JS：解构默认值
来源：http://hz.zhongyouzk.top/gtxnqyxmdq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtkcdxsnxe.html

[U88] JS：对象展开合并
来源：http://hz.jyoumei.cn/gtzksfvnqg.html

{ ...a, ...b }
来源：http://hz.yuanzhike.top/gtatutwshh.html

[U89] JS：数组去重
来源：http://hz.zhixingplan.top/gtxvozgtva.html

[...new Set(arr)]
来源：http://hz.jianghu66.top/gthcpjqiay.html

[U90] JS：数字数组排序
来源：http://hz.cashguo.top/gtkdngmgxf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtnqilomor.html

[U91] JS：对象键值遍历
来源：http://hz.iojbl.cn/gtolhuhpir.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jlsjyb.cn/gtanjkhqaa.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gtfkujrbfh.html

structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtuwnfqjtl.html

[U93] JS：模板字符串
来源：http://hz.tanke756.top/gtxyfpknep.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gttvaieivf.html

[U94] JS：箭头函数
来源：http://hz.aizwys.cn/gtyyhdgmau.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtephhxzdf.html

[U95] JS：Promise 包装
来源：http://hz.hysaishi.cn/gtdkxlejyp.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gthzjbrazk.html

[U96] JS：async/await 与异常
来源：http://hz.shuidangran.top/gtqfhmpozx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtdyargpii.html

[U97] JS：并发请求
来源：http://hz.wangdashe.top/gtbeilejyp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtdwaabdnz.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydjk.org.cn/gtbseffmxm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tanke756.top/gtqlbzviyy.html

[U99] JS：事件监听
来源：http://hz.ehwqpu.com/gtzhaohjtw.html

el.addEventListener("click", e => {})
来源：http://hz.tianlin.xyz/gtjgxrecaj.html

[U100] JS：DOM 查询
来源：http://hz.ydzc1.top/gtqlmchhsb.html

document.querySelector(".item")
来源：http://hz.smart0.xyz/gtmxowycwh.html

[U101] JS：classList 操作
来源：http://hz.c1oappe.top/gtwvdihgiv.html

el.classList.toggle("active")
来源：http://hz.jinghuilouyu.cn/gtqltdqlyk.html

[U102] JS：本地存储
来源：http://hz.jinghuilouyu.cn/gtxzgbbuvf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtfozekhaf.html

[U103] JS：定时器
来源：http://hz.9152youxi.cn/gtwlnpwvbk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj20258.top/gtdplxmada.html

[U104] JS：防抖
来源：http://hz.sweek.top/gtkuzjogtp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtsfyyveaw.html

[U105] JS：节流
来源：http://hz.fengsongda.top/gtotfelpcv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.redwolf501.top/gturskzrdq.html

[U106] JS：日期格式化
来源：http://hz.hammf.cn/gthlvbclbd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guannengcc.top/gtkfccnqvs.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtefwplfvf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sufxvd.cn/gtwpzopywq.html

[U108] JS：随机整数
来源：http://hz.wangdashe.top/gtvgutwpfv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtndfjgpbe.html

[U109] JS：数组分组
来源：http://hz.0kj1m.cn/gtsitzrhae.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtfcddxulx.html

[U110] JS：数组分块
来源：http://hz.nwbrower.top/gtaieergpb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj202588.top/gtreklgbeu.html

[U111] JS：对象转 Map
来源：http://hz.quarkkingdee.top/gtrsdzplgk.html

new Map(Object.entries(obj))
来源：http://hz.feifeiyinyue.top/gtnnjlldae.html

[U112] JS：字符串补位
来源：http://hz.zdqjudy.top/gtireeyttl.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gterwszzgh.html

[U113] JS：正则替换全部
来源：http://hz.feifeiyinyue.top/gthzxzjsxa.html

s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtaebgfljz.html

[U114] JS：JSON 深比较
来源：http://hz.yvedp.cn/gtjwwohdem.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtlaolakcy.html

[U115] JS：生成 UUID
来源：http://hz.hfpthk.cn/gtqbkibajn.html

crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtikaxztwb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.vqdsnc.cn/gtifrrrzdb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tianlin.xyz/gtiqdfnjjq.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtwbalbgzg.html

npm i -D vitest;  npx vitest
来源：http://hz.zycfv.cn/gtwtlndlzt.html

[U118] JS：开发服务器
来源：http://hz.yanxiufei.cn/gtuqkrpcxn.html

npm i -D vite;  npx vite
来源：http://hz.jianghu66.top/gtduzknhxx.html

[U119] JS：生产构建
来源：http://hz.gogol.net.cn/gtpxopeann.html

npx vite build
来源：http://hz.yuxming.cn/gtxxmrmpsx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ivvv.top/gtpyevgida.html

import.meta.env.VITE_API_URL
来源：http://hz.xziqi.cn/gtrcsbnrgn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdysqenes.html

统计汇总
来源：http://hz.ivvv.top/gtirxowuyr.html

================================================================================
来源：http://hz.yvedp.cn/gtyxuqkxpj.html

按语言统计（条）：
来源：http://hz.jqgufenzy.top/gtynhsibpv.html

Python ......... 252
来源：http://hz.hnxiangtu.top/gtackgexgj.html

PHP ............ 252
来源：http://hz.zycfv.cn/gtkjonkxjp.html

JavaScript ..... 252
来源：http://hz.jinqigufen.top/gtzuwgurys.html

TypeScript ..... 212
来源：http://hz.yanxiufei.cn/gtjqexznwz.html

Java ........... 212
来源：http://hz.wangdashe.top/gtzqbcgqig.html

Go ............. 212
来源：http://hz.yangfankeji.com/gtsswlbrzg.html

Ruby ........... 212
来源：http://hz.zdqjudy.top/gtsqwpclle.html

C# ............. 212
来源：http://hz.zhongyouzk.top/gtyswdcwkz.html

C .............. 30
来源：http://hz.andypj.xyz/gtquxdmnkz.html

C++ ............ 30
来源：http://hz.tanke756.top/gtrkwkvmzf.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtznfnkboi.html

Bash ........... 80
来源：http://hz.jinqigfzy.top/gtmbyjwgsy.html

Kotlin ......... 15
来源：http://hz.jianghu66.top/gtvyhypyqh.html

Swift .......... 15
来源：http://hz.smart0.xyz/gthpjtqbbo.html

Lua ............ 10
来源：http://hz.chenjidiqi.icu/gtyzjkqegb.html

Perl ........... 10
来源：http://hz.yueranfly.top/gtmsqtsjuq.html

Scala .......... 10
来源：http://hz.fzhhl.top/gtqrvohddk.html

------------------------------------
来源：http://hz.0kj1m.cn/gtlbgsmtgd.html

合计 ........... 2106 条
来源：http://hz.xuetiantiany.cn/gtaygnjmip.html

按章节统计：
来源：http://hz.zhengqikj.top/gttvedktxr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtvgpnyqgq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gttbrcceva.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtksqbsdsq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gthzeldfxi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yangfankeji.com/gtprvrobfd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtelknxnll.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gtxiywjdeo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtfvqjovtm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtvhvnujvy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shzxlz.cn/gtoszziltd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gteznielkm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gteflwgsle.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtqdpfnncb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhijiandao.cn/gtyqfekqhp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gaohongyu789.top/gtvhjjipnj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtltldcicp.html

Q SQL 专题                              90
来源：http://hz.jinqigfzy.top/gtheuuozri.html

R Bash 专题                             80
来源：http://hz.jiagoushi.top/gtfhqlixgi.html

S C / C++ 专题                          60
来源：http://hz.hfpthk.cn/gtaazttbrk.html

T 其他语言补充                          60
来源：http://hz.hnqzz.top/gtbkmzrhjo.html

U 高频实用片段                         120
来源：http://hz.smart0.xyz/gtreitwwhk.html

------------------------------------
来源：http://hz.gaohongyu789.top/gtqecfoigq.html

合计                                  2106 条
来源：http://hz.9152youxi.cn/gtcxrryofp.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtewogtfrf.html

使用提醒
来源：http://hz.haohaochexian.top/gtyrgoqpyd.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtoveszsfb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sweek.top/gtezhkwkan.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangkeji.top/gtezaravpn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258888.top/gtefqaamxl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.redwolf501.top/gtkcqqljfd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tianlin.xyz/gtlwjvxgjd.html

—— 文件结束 ——
来源：http://hz.hysaishi.cn/gtqcppvuds.html


<!-- 参考信息 -->