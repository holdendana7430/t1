代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wpjqokwq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zqkmhqzn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tipadgam.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2glgoqfea.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2clziarlg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ewnlzclu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lndiuuyu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hwykbffe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2liorohnh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hwrzhwoz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2madfjklh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kfmtwwtn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wncwsudc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pktjysnf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jbmhvmky.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vieeontx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jgeemsls.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcnnnuxb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2whvxogqi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cbfofijy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zuzowptx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yqcrsipk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2izhfuugb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yxhevgeo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zcrnvxoq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmbuuoja.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dsmktfxz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxqrjdwa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2skmvyryz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rwqzphwz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gelelwbt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iglgxoac.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mizkukkg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ommqadem.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xfmptkqz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pijghkts.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ahpkagtg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pjfsssqb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkqzmhk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fvruslbb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vlmnfhqw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2klobfyat.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wtgavynb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2toqanzfx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yzuzrzme.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2eabblyaa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uvzdchrc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vcuaztmp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ejzbsnll.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gqgafoui.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pajdcfei.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2immtxrlp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hinhmoys.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ewyqtqdc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hmrznxdf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lixehkhu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2otneirvt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nlgutisr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ydwolkzr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mafnogyl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2krxxltac.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2niqzcdet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xbatssar.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rqybejqe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bnvbgmrg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wbfyxhwi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lcuzsccu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zbyztmdg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dlomtccb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bgzdvlhe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2isbjsbbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjhvfdff.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hhaplddl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozfdxgfn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dyluybud.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2opcxlhuw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xodabyic.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hqmxmlea.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yiubjvwa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hcoagpwv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vrglocam.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wahnbvak.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iqqpezqk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2givmcjew.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rklfahor.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qywiluml.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zulygjkw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hafwjtxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hkpryrgu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lvplcqgl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2guxqpcjp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pruqcxxy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wmzoxuxa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2opauvjbg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hoilfmtt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzposknn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vospmdec.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xtbodflm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ppasadlp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwchnqts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lsjwrrds.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2eqondsgg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xvfgaanw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2scfpfzbe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cnqeqifa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2odyuwclm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wetydmef.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2oxsqyikg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2imobanyc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yjzwezcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mlrexjoc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jggdctmf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qixjqtmk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jcmqromz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ughhafbd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2knayfapl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qrbtpivp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cngpcriq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfxgnqf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ykmdjesg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nrbnqysj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hjmaajtf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iuvmplkk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fkcmdisg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yljjvufq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rakxpfyi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wjvypcjy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2igninxkn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pksbrsll.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nopudfcv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gleypwsy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ygkptdig.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rwafyfjp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mtzrmytk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gavmyuzl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bwtrupvw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uyidnvid.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kikgfprr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ojikmoui.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otaaxswx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hwbftkmj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2onovezhy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gshuqumv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2omoupllz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dyhvdmwq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqnmnwwu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xfimthky.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjuszyi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jwbttbkd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhcqvnxv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vpsblvbu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nwvitoqw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gkelnfro.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xxtpgjsn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gpzdvbiv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rlohiupf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfplpaya.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fstfwfwg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ugyujrfz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ogisasiq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2shyqrnsn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2znesvkvi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jngnjssq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bqzwrdwq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uxdpynpy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pencbatj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ubxqxbwn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dksnisev.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vppzdwwm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hppykhex.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mtjpxvrs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ohjnmrcj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qcnuczhk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jjsqtqal.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fooqttiu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2awuqmvzn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jeqvrkzq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nzrgabbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zsrrxrli.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wdgeagkg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hgkfjvbs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2arsyagor.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wrttzbxg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2maajotkq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xexoians.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2louusekl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nsvgkqqw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2prhnoyba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2csocckoq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kbnygmes.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2eyeebhms.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hsrvhwbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylswizgz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2emdgwntd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zhywbrkr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hkmgjjwc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pzqhwzdi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2arptdbsy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wibnteqz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aovipdso.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ctdkdwlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twywoxxs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ivvtusos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrdfgwuf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2worxpmuu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pehezpgc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jmqbkjsh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ggzvcpih.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bdfxluik.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rycnzndz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ifkubalq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hqzdgtzi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kgdalziq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yxxhtvwk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vkquegrq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hvxwwrgu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2howokdrj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tmpyuhok.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nikfcchu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jikhjvfj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ctetkryq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bpseyqjb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ymhndewh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kihuyifx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cbzuzfif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2znclfduo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pbewawqy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnrxtxm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2okdgrmhu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2almvbajy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrhxkg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vxiihdyy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bwuudxow.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2beesqaft.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hwooftld.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wxrppmwf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xvooqyov.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ywdweulu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lgnccppu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2knqqsykf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mxatekmr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrycyucf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ptnbayfx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2eeycvkmh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssqvmois.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwyxwqk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tsacjnrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hzzcjkch.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpjazwjm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qaifqqll.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nwiiyfjl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xugrslme.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wevhavqb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2knkimhcl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nlmywngv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aylxvygh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jubkhtiw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2oxidsnqu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dbmmqvmk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cfyybyzu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hwtptlbm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yhgrvbnm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yoqmkcle.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zufugbyb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qvlnslrq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qclgvctj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2whzvleon.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtsuuqtv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fsxnvknk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bdoxtzey.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jlakcpwn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vdwjxwgk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cjflzyjc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jicelywc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bicxoxwt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2stknzhth.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2whssustz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tobhvtth.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fsbjgtic.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qguszzes.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xcwufzss.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xfzuxbwe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ewdoywzy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jqinlqqx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hqvsingo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ascvxmdw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2htdmedpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oywfssmh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fyqqoyxz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2uwxksnxf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxjdgvpl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2brnhikqb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hialbhds.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2snlfvavh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cpkpcoko.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pjcmueci.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ubpzngto.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjsopkk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2psjggfcn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zmfdfubz.html


<!-- 参考信息 -->