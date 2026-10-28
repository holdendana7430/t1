代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtitjjmnse.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gtqmarywco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gtjunexpbf.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gteyyizezn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtewqtqnmq.html

[R48] awk 取指定列
来源：http://hz.dashuyun.cn/gtvtgwlgwv.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtgixzmqeo.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtglonaese.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gttmiyyhgb.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtaebdkzgx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yonumen.top/gtjryegbzj.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtveggfgel.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yangfankeji.com/gtlrtdlhbc.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtwerptyeq.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtwfsbgljd.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtxsuilxsf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtmtvltcqv.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtlnjtymhi.html

diff a.txt b.txt
来源：http://hz.jinqigfzy.top/gtdtlzyygd.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtqallrppq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gthimmtgee.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtzdbszejp.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtqqkxdkgk.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gthpurubno.html

ssh user@host 'uptime'
来源：http://hz.52xcode.cn/gtlqehbqdb.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtmdnvofso.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtxitltfqk.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtxkroxxem.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtiojgwdag.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gtukuwoooq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gthbljllxh.html

[R61] 磁盘占用
来源：http://hz.nanxuanxn.top/gtimlzfllv.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtjeoqiwls.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtbrijbvrl.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtrrkljjrp.html

[R63] 内存与进程
来源：http://hz.ybcxt.top/gtwfrdlyyd.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtuumgomqw.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtjshiednr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtcqpkpsvl.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtripckwxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtnzdoqvnj.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gtjenurkqe.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtucovthyg.html

[R67] 生成随机十六进制串
来源：http://hz.chenlongwang.top/gtpuevxmjk.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtjboaojnw.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtkblkwapd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtkbtikfyb.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtrerjrdyh.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtejfgotvv.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtuehjxhkl.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtlnmxhgst.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtcazfiswe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.52xcode.cn/gtyawjzagv.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtfiflrige.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtdhiklfys.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtltwbyidy.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtnojrhqat.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtnlrvawbt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yangfankeji.com/gthcoeixzm.html

[R75] 导出环境变量
来源：http://hz.9152youxi.cn/gtwcxeilza.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtjfxofxef.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtfwcpnoqr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtheyxiljr.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtpuetbtdq.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtjhemprae.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtswifhadp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dashuyun.cn/gtepvujxqw.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtlcdynkzx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtsxuobwjr.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtuyvknonu.html

time ./run.sh
来源：http://hz.yj20258888.top/gtpsupkkmn.html

================================================================================
来源：http://hz.wangdashe.top/gtnfyducnr.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtgnyukwlr.html

================================================================================
来源：http://hz.kuanghao11.cn/gttdbpsqve.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtufrrteai.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtdjkyzlxg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tian-w.cn/gtdrcihrnf.html

[S02] C：变量与格式化输出
来源：http://hz.hongshengwenyu.top/gtjfdjlakk.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtgfadsumb.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtgprrcqmq.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtivvwpvqs.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtaqntmtsu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shuidangran.top/gtvxfwyyrd.html

[S05] C：字符串长度
来源：http://hz.tian-w.cn/gttlnjqisx.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtqrpeupvo.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtfimzgzpv.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtfpemtluh.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gttztipzzq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtcepqclqq.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gtexxompfg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fzhhl.top/gtmfhjafiy.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gtqnagdxrm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.52xcode.cn/gtjhmcausn.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtfoxnoaka.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtpicblbkz.html

[S11] C：逐行读文件
来源：http://hz.yvedp.cn/gtvxhfmkiu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtorpqnkmn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtmftlqsxa.html

fclose(f);
来源：http://hz.havefunace.top/gtlxebycqf.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtbipkkdht.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtoptdierq.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtjhkkgiim.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtnmxytpty.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtljmkvgpe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuanzx.com/gtkdlcxnag.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtazmdndck.html

(double) a / b
来源：http://hz.hfpthk.cn/gtrtiapjjv.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtqaepybjg.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtxsfpirqi.html

[S17] C：安全拼接字符串
来源：http://hz.daria6918.cn/gteoqeauqr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtnsutogds.html

[S18] C：命令行参数
来源：http://hz.sweek.top/gtdflnfybx.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gthmmrshhs.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gtshycytil.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtagquixjq.html

[S20] C：二分查找
来源：http://hz.aizwys.cn/gtofdvymok.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtyemxoznn.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtfdrwanhe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtdhffiboe.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gtcjovaman.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xingfuxueyuan.xyz/gthcyiitys.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtcbwddhkf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hysaishi.cn/gtvuztwbdn.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtvjcxcowh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtjbdgeiwf.html

[S25] C：内存拷贝
来源：http://hz.nanxinkj.top/gtnumzxzkw.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtszsptmsy.html

[S26] C：内存清零
来源：http://hz.tanke756.top/gtqdsqduaq.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtnkdyusuc.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtmzlzjqft.html

const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtbiuyzejq.html

[S28] C：静态变量
来源：http://hz.tian-w.cn/gtlzxyllkt.html

static int counter = 0;
来源：http://hz.tanke756.top/gtjbzndtec.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtvituaiej.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtldlaufme.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtelzugwwj.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtegmfcbrc.html

#define X_H
来源：http://hz.cqqwz.cn/gteykozeto.html

#endif
来源：http://hz.shangyingyoupin.top/gtyasehuqc.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtsgvfyslf.html

#include <iostream>
来源：http://hz.smart0.xyz/gtcyxbhgzi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.pengpengdd.cyou/gtlsaedkpa.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtvsxobqyl.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangkeji.top/gtxooaxwjs.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtuulhdowg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtrjaxnbda.html

[S34] C++：遍历 vector
来源：http://hz.meibo888.top/gtrgvrugli.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtmcdpmlpd.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtsbrfnack.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtglsjylld.html

[S36] C++：unordered_map
来源：http://hz.xingfuxueyuan.xyz/gtigukgniv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtgxmzygle.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtemsuturo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtqsvjlmgw.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtidnngpqn.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtjtvklsib.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtsdibgkip.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtvinrqpzs.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtirlpivce.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtancobdwq.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtibqjrmug.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gthgdfjoah.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gthofxqvkl.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtdxvatfaf.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtfysdltqo.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtwsyexfeo.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtmoskqthy.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gthjjbjocf.html

[S45] C++：lambda
来源：http://hz.yj20258.top/gthnnxsosi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtsafxnrsv.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtjkauwbaj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtzeajgvev.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenlongwang.top/gtdcwhhiim.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gteneufzfr.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtwyovlpik.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtclxnmkix.html

while (std::getline(in, line)) { }
来源：http://hz.ybcxt.top/gtnfqndkyj.html

[S49] C++：写文件
来源：http://hz.sweek.top/gtuolflfvg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtfultzdqf.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gtbxleubtg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtazshgpaw.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtrogsmaet.html

static_cast<double>(a) / b
来源：http://hz.chenlongwang.top/gtsjivlseh.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtzhjegity.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtazscogwt.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtzffhevie.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtveyofbls.html

[S54] C++：异常处理
来源：http://hz.zdqjudy.top/gtforhgewd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtqxixwwkn.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtpmgqqhbq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtnytbvhsa.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtmplmdbds.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.mhx1999.top/gtknlcyfwr.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtwowvecsx.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtkurviugo.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtwmngcdnd.html

namespace ns { int f() { return 1; } }
来源：http://hz.gotoacloud.top/gtsrkgyvzc.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtgkbanpsn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.redwolf501.top/gtsozxunnm.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtxzbzrgvb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtilabiuaq.html

================================================================================
来源：http://hz.yueranfly.top/gtbcbaresw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gttxfnqngk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtshzkgbpt.html

[T01] Kotlin：Hello World
来源：http://hz.iojbl.cn/gtnkkwerhl.html

println("Hello")
来源：http://hz.sufxvd.cn/gtzmdcevhh.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtqaxisqez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtdrlyosbr.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtdjvzohib.html

"值: $b"
来源：http://hz.tianlin.xyz/gtgeszvgxg.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtussvzlqp.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtjestgkkp.html

[T05] Kotlin：when 表达式
来源：http://hz.aibaodan.cn/gtfnslevtf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtumtfedwb.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gtqfkrxrqb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fzhhl.top/gtfgfkawla.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtcqacgrcz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtileyoion.html

[T08] Kotlin：数据类
来源：http://hz.quarkkingdee.top/gtwfgkbqzt.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gthnlkmhki.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtkejnunde.html

fun String.exclaim() = this + "!"
来源：http://hz.yuxming.cn/gtlybfogha.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtsmnivsey.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxuanxn.top/gtguxjxvqm.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtnbsncqlc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cucudq.cn/gtzxnyxvll.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gtfjpptthz.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinqigfzy.top/gtwmgljtmb.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gthucobuoy.html

val m = mapOf("a" to 1)
来源：http://hz.fzhhl.top/gtmpntsofm.html

[T14] Kotlin：循环
来源：http://hz.ydjk.org.cn/gtiebvlshh.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtzzfyejih.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gteshdkrzf.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtdlehltei.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtctvelrxm.html

print("Hello")
来源：http://hz.shuidangran.top/gtzpozlroe.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gtokaqoihz.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtclaivtee.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtxisoyvpr.html

"值: \(b)"
来源：http://hz.yanxiufei.cn/gthfcblqnn.html

[T19] Swift：可选绑定
来源：http://hz.hnxiangtu.top/gtdfgowyau.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtyauokfpg.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gtovlzmfja.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtjxyepvfu.html

[T21] Swift：遍历
来源：http://hz.gogol.net.cn/gtsoiqmtqh.html

for x in a { print(x) }
来源：http://hz.ydzc1.top/gtechvkxds.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gtuqrrbadb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtbqsosott.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtbgtzhxlc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.havefunace.top/gtdyjfnlor.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtxtpzrwsh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gtohoiehhb.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gthltuyndu.html

struct P { var x: Int }
来源：http://hz.fzhhl.top/gtfommpmhr.html

[T26] Swift：类与重写
来源：http://hz.zhongyouzk.top/gtkaedeygj.html

class A: Base { override func f() {} }
来源：http://hz.tanke756.top/gtlqizupjs.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtasuywmko.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtptxwdpvu.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtnlrmboea.html

enum Color { case red, green }
来源：http://hz.zhijiandao.cn/gtvlxlvwlm.html

[T29] Swift：guard 提前返回
来源：http://hz.mhx1999.top/gtajiyrkbd.html

guard let x = opt else { return }
来源：http://hz.0kj1m.cn/gtbfvclwiz.html

[T30] Swift：协议
来源：http://hz.daxiang520.top/gtydpwwcsv.html

protocol Shape { func area() -> Double }
来源：http://hz.zhongyouzk.top/gthlgnzixv.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtawaoefvm.html

print("Hello")
来源：http://hz.yonumen.top/gtjdbbhbpl.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtoencckjl.html

local a = 1
来源：http://hz.nanxinkj.top/gtwokwhoed.html

[T33] Lua：表（数组）
来源：http://hz.ybcxt.top/gtxqxtlmuz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.mhx1999.top/gtemzbbgzh.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtgjtggnyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sxryk.cn/gtanyuzasg.html

[T35] Lua：字典表
来源：http://hz.shuidangran.top/gtbltupnoi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gtjlzsijvi.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gteznrsbrj.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gteccfldad.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtfpusgrrx.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtgiiksblz.html

[T38] Lua：条件
来源：http://hz.guannengcc.top/gthhayefaf.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtatmawfpx.html

[T39] Lua：模式匹配
来源：http://hz.meibo888.top/gtiipwygvd.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gttjfqhsbu.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gttwfkrllz.html

setmetatable({}, { __index = base })
来源：http://hz.zhengqikj.top/gtrbxsxvis.html

[T41] Perl：Hello World
来源：http://hz.gzhubu.top/gtsjxegnad.html

print "Hello\n";
来源：http://hz.yvedp.cn/gthcrmsita.html

[T42] Perl：变量类型
来源：http://hz.guannengcc.top/gtixhaumtk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtazgcqnpv.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtlsllvymo.html

"值: $a"
来源：http://hz.fzhhl.top/gtpbeoabej.html

[T44] Perl：条件
来源：http://hz.nwbrower.top/gtlnkfcryy.html

if ($a > 0) { print "正"; }
来源：http://hz.fzhhl.top/gtzbjrpmhv.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtqxwkgvuq.html

for my $x (@arr) { print $x; }
来源：http://hz.zdqjudy.top/gtzuyiywks.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtolrjvxip.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yanxiufei.cn/gtfdnekftu.html

[T47] Perl：正则捕获
来源：http://hz.xuetiantiany.cn/gtibusakxu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtoearrvsa.html

[T48] Perl：正则替换
来源：http://hz.zhaomingkeji.xyz/gtbkypjbfk.html

$s =~ s/old/new/g;
来源：http://hz.yj20258.top/gtcihnfxcj.html


<!-- 参考信息 -->