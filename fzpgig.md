代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtbogygalp.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gtaohqzalg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yonumen.top/gtdkgesljs.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtyjvxsimt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtrdljawtj.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtcfwtzjwv.html

awk '{print $1, $3}' a.txt
来源：http://hz.sysykeji.top/gtoqtnrkup.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtvunyuepc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dashuyun.cn/gtsuaanwzm.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtejwqswsn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtlmekoqig.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gthdckmeod.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtuczdyutz.html

[R52] 统计行数
来源：http://hz.jiagoushi.top/gtirojtisf.html

wc -l a.txt
来源：http://hz.yongpay.top/gtmxjanjfi.html

[R53] 查看文件头与实时尾
来源：http://hz.mhx1999.top/gtodwrtyoc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.316326.xyz/gtcivclqkr.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gthanfxgld.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtzbsjjnwv.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtixowphnk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtnbkppzop.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtgmhjbvdi.html

scp file user@host:/path/
来源：http://hz.yanxiufei.cn/gtolkzmhgg.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gthxhvdgvz.html

ssh user@host 'uptime'
来源：http://hz.0kj1m.cn/gtxgoosnli.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gttqgcataj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtdrjbocwy.html

[R59] 发 POST JSON
来源：http://hz.0kj1m.cn/gtyielpvbl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258.top/gtafmjbdgm.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtzelicbjh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtpintpbwt.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtodbavihi.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gttcmoimwo.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtaqnbvgkv.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gtuutmmmbz.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtkuazhbbt.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtzwfgtdkh.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtghokitsq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gtfkcazwfh.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtcifcchzw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnxiangtu.top/gtyyitvmht.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtqnswjgkg.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtpdxnkwnf.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtukyehnmh.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtmokhzbis.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gtlndbgctq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtccjlimxf.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtdluvckzl.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtwkllrhlp.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtseydyvtt.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtlwfpxyoc.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gturyieylb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtyrmlfbeu.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtbyguyqqg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtadrtcdeo.html

[R73] 分割大日志
来源：http://hz.hnqzz.top/gtgtmouvog.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gtojvhqrcr.html

[R74] 批量重命名
来源：http://hz.yvedp.cn/gtnpyfneap.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtycjardrk.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtgmxdsdef.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtqmariciw.html

[R76] 使用临时文件
来源：http://hz.zhoulong.xyz/gtuwihydhd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtlgamxzav.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtwjfursqa.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtvqumegsl.html

[R78] 交互式菜单
来源：http://hz.jinyuanbaomall.cn/gtdffvnygi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtmmlznxnh.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gttndkeivk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gttnofttjm.html

[R80] 查看脚本执行耗时
来源：http://hz.yanxiufei.cn/gtlbsbudju.html

time ./run.sh
来源：http://hz.nwbrower.top/gtovkuabib.html

================================================================================
来源：http://hz.ehwqpu.com/gtkkipscoj.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtvuudnwds.html

================================================================================
来源：http://hz.haohaochexian.top/gtaigwskxy.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtmduaarzo.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gtjqfojiys.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtexkkrrwe.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gthsxfiksb.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtlbylzvnf.html

[S03] C：读入整数
来源：http://hz.xinyue.icu/gtpnijekjy.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtrrgjveal.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtkxqiaclg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtxwafhehd.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gtliicbqcs.html

strlen(s)
来源：http://hz.52xcode.cn/gtxmpzsoxm.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtpmuamnyz.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtehlynwif.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gtezlfmccz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.svipenyu.cn/gtcjmrubxd.html

[S08] C：动态内存分配与释放
来源：http://hz.zhiwuduotai.top/gtcrecyhzy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtoqowkstq.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gtkivydlrd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtzizgaitm.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gthdvkwfkp.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gttfxrnnxd.html

[S11] C：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gtursvflbp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cashguo.top/gtjaajedmv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gtnsjxrqrd.html

fclose(f);
来源：http://hz.ydzc1.top/gtmrkrahrg.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtgcipjpiy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gteafnptkg.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gtwtpsvmkp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtaxjyeoao.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtyetitotk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtxgwkglfe.html

[S15] C：类型转换
来源：http://hz.0kj1m.cn/gtlldwneqr.html

(double) a / b
来源：http://hz.birdmap.top/gtmfoxnbks.html

[S16] C：位操作置位
来源：http://hz.xylfe.cn/gtvwdtprkj.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtqwotcrwl.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtbmutkwin.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtxrsrdjsm.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gtlgapudpl.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtdzmjrqsg.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtpjwrgoyx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtsjkapfpb.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtkixwwqge.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtbppjucob.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gtshpmnyuj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtpwgrrvjy.html

[S22] C：字符串转数字
来源：http://hz.chenjidiqi.icu/gtxneaynlb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gtlltrpycb.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gtokewyuxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtdynxpbsu.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtpjiglayk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtjasqjqso.html

[S25] C：内存拷贝
来源：http://hz.ydzc1.top/gttcsgopcj.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtutywbkbb.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtetnaixzp.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtyjvzourx.html

[S27] C：定义常量
来源：http://hz.sxryk.cn/gtcygitvyk.html

const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtthkzqfiu.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtodkowscu.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtspwhahjf.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtbbdqpufo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtewstuche.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gttotaxtaj.html

#ifndef X_H
来源：http://hz.316326.xyz/gtwwiebacv.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gtpuvwguia.html

#endif
来源：http://hz.aizwys.cn/gttfmxaceq.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtsqharcro.html

#include <iostream>
来源：http://hz.jlsjyb.cn/gtrfqrtuoy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtioweimkp.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtjxxfoexy.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtrxqaxwfd.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtkolzzhsu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtisseozpc.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtcplnfbxv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtnldvdrua.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtbkgmtvxy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtnabhgjql.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtpmqbzhvn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtgrxmhdtk.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtvacpczzl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtsvighfxd.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gtvpeyqszr.html

std::sort(v.begin(), v.end());
来源：http://hz.andypj.xyz/gtrparbvph.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtwhkdizyw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtzkmsbgfp.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtumajacbc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fzhhl.top/gtpoiruxuf.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtmkjdagxc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.andypj.xyz/gtvdgsqzhn.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtocmxunoo.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtjuitujst.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtqinnczce.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtoibihgyj.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtxyiypqjc.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtqybebbuy.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtorpbtdrp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgfzy.top/gtpsbwyfjn.html

[S46] C++：函数模板
来源：http://hz.yj20258888.top/gtnpvasldx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtanllhtva.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtxxxxjuko.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtvlmjdelf.html

[S48] C++：逐行读文件
来源：http://hz.bjfxy.top/gttupktfun.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.bjfxy.top/gtjqencvjh.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtzkeszmvy.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtnbbxxkjc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgufenzy.top/gtnlmwhgjh.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtybzqlfhr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtskgcdeiw.html

[S51] C++：显式类型转换
来源：http://hz.gaohongyu789.top/gtpybfvtiz.html

static_cast<double>(a) / b
来源：http://hz.yj20258888.top/gtjyzkubxq.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtekjegsxh.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtrmyqueyd.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtvbfppptf.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtilppewkg.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gtodgawyeq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtlsxnwslw.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtpyvgfezb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gthqxrrdxg.html

[S56] C++：optional
来源：http://hz.yonumen.top/gtrkacbwtf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gtgekkvbji.html

[S57] C++：编译期常量
来源：http://hz.jlsjyb.cn/gtpvfnhkwe.html

constexpr int N = 10;
来源：http://hz.yueranfly.top/gtesnsagcy.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtnhoqgpmh.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtbeexawad.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gtewpebojd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtttvcyupy.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gthqejwwsp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtiezdzbvn.html

================================================================================
来源：http://hz.xuanzx.com/gtrboxhaur.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gtvgipwgjz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvddpmnis.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtzurprnvz.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtbhtaxytu.html

[T02] Kotlin：变量
来源：http://hz.birdmap.top/gtihhwstqg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtlcdotcgz.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gttgglpvrs.html

"值: $b"
来源：http://hz.kuanghao11.cn/gtdtesoaso.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtnuujrhkx.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtgkymsawg.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtjxomzedn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhiwuduotai.top/gtbuvndioa.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtdwyweina.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gtmjhwlroa.html

[T07] Kotlin：集合过滤
来源：http://hz.jiagoushi.top/gtjgriuwpc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtaqysgicg.html

[T08] Kotlin：数据类
来源：http://hz.ydjk.org.cn/gtblacbkql.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gtzhbvcxdz.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtudapewwz.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtzddgkfna.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gtukyxxhsq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtwzaoqevh.html

[T11] Kotlin：协程
来源：http://hz.shangyingyoupin.top/gtnkplghtg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtdrpjapmu.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gtndgudqfn.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtgrreahpx.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtfunxfwjj.html

val m = mapOf("a" to 1)
来源：http://hz.guowangkeji.top/gtwvevtitu.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtubxifhhd.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtjutltgdj.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtpkwkndhj.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtxaaoghoq.html

[T16] Swift：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtqpmxjbvn.html

print("Hello")
来源：http://hz.yueranfly.top/gtckwemtdg.html

[T17] Swift：变量与常量
来源：http://hz.yj202588.top/gtzklnwdvv.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gttsgrsfjp.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtedczmjnq.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtvxjwvzfx.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtmvlibfna.html

if let n = opt { print(n) }
来源：http://hz.haohaochexian.top/gtemknzbzg.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtujkzhmgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtlqgfubso.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtvaaztiko.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtxtwasdye.html

[T22] Swift：字典
来源：http://hz.tanke756.top/gtqejmjubq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtccwhiplh.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtrhsaeuzq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtlkaeqdnl.html

[T24] Swift：闭包
来源：http://hz.smart0.xyz/gtpxbklhiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gtmssvloho.html

[T25] Swift：结构体
来源：http://hz.smart0.xyz/gtbmeupcsw.html

struct P { var x: Int }
来源：http://hz.tianlin.xyz/gtvoglusjz.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gticqshvwv.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtbykuchyz.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gtvglgpjvl.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtuudqhmvl.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtmyjsijrr.html

enum Color { case red, green }
来源：http://hz.xuetiantiany.cn/gtgskmzxpo.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gtyojhgnji.html

guard let x = opt else { return }
来源：http://hz.gaohongyu789.top/gtqxrusqbs.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gteqgqjisa.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gtclemjvpg.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtnphhtucn.html

print("Hello")
来源：http://hz.xinyue.icu/gtoqtycmsc.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtefxmkbrq.html

local a = 1
来源：http://hz.ywan-chungtsiang.top/gtydknavyk.html

[T33] Lua：表（数组）
来源：http://hz.fzhhl.top/gtzxsnhapn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuanzhike.top/gtkrqfecba.html

[T34] Lua：遍历表
来源：http://hz.yanxiufei.cn/gthffsrkqc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtjdjbxdzz.html

[T35] Lua：字典表
来源：http://hz.xuetiantiany.cn/gtdkkgynrp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtyawngykx.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gtjcuiuvod.html

function add(a, b) return a + b end
来源：http://hz.xuetiantiany.cn/gtmslmjunv.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtxfzffvro.html

"a" .. "b"
来源：http://hz.yanxiufei.cn/gtpukbuftl.html

[T38] Lua：条件
来源：http://hz.316326.xyz/gtyvamryny.html

if x > 0 then print("正") end
来源：http://hz.ehwqpu.com/gtnilrlxdw.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtabnelcrq.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtzlmtbybg.html

[T40] Lua：元表
来源：http://hz.feifeiyinyue.top/gtxwnsyprs.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtfkzyhxdh.html

[T41] Perl：Hello World
来源：http://hz.nanxuanxn.top/gttsjgpmpd.html

print "Hello\n";
来源：http://hz.jinqigufen.top/gtmlbwjmyh.html

[T42] Perl：变量类型
来源：http://hz.chenjidiqi.icu/gtjuapcfms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtfltbjnjo.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtjpghcllc.html

"值: $a"
来源：http://hz.jinghuilouyu.cn/gtvqiebuph.html

[T44] Perl：条件
来源：http://hz.hywenlv.cn/gtdrpqihks.html

if ($a > 0) { print "正"; }
来源：http://hz.ydjk.org.cn/gtmggkeodm.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtfwltdmax.html

for my $x (@arr) { print $x; }
来源：http://hz.hongshengwenyu.top/gtcccrdmlt.html

[T46] Perl：哈希操作
来源：http://hz.vqdsnc.cn/gtejinkotp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ybcxt.top/gttavrvljz.html

[T47] Perl：正则捕获
来源：http://hz.zhixingplan.top/gtwjintvqf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ivvv.top/gtstsoxpmz.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtxshcsxnk.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtguilvgyb.html


<!-- 参考信息 -->